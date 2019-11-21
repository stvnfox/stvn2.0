<template>
  <v-container class="mb-12">
    <label for="project" class="projects__title headline text-uppercase">
      Projecten
    </label>
    <v-row id="project" class="projects blue" align="center" no-gutters>
      <v-col class="headline text-center">
        Hier een lijst met projecten die ik heb gemaakt
      </v-col>
    </v-row>
    <v-row no-gutters>
      <v-col :key="project.id" v-for="(project, index) in projects" :class="index === 1 ? 'blue lighten-4' : 'blue lighten-2 white--text'" cols="6">
        <section class="pa-12 text-center">
          <h3>{{ project.title }}</h3>
          <span>{{ project.subtitle }}</span>
        </section>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  props: {
    projects: {
      type: Array,
      default: () => [
        {
          id: '1',
          title: 'Project titel',
          subtitle: 'Project ondertitel',
          bg: 'red'
        },
        {
          id: '2',
          title: 'Project titel',
          subtitle: 'Project ondertitel'
        }
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
  .projects
    height: 40vh

    &__title
      position: relative
      top: 8px
      left: -2px
</style>
