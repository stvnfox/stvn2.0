<template>
  <section class="mx-10">
    <v-container class="heading">
      <div class="heading__text">
        <v-row>
          <v-col tag="h1" class="text-center text-uppercase">
            Steven Vos
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col class="headline text-center">
            Ik bouw digitale producten
          </v-col>
        </v-row>
      </div>
    </v-container>
    <projects />
  </section>
</template>

<script>
import Projects from '~/components/index/Projects'

export default {
  components: {
    Projects
  }
}
</script>

<style lang="sass" scoped>
  .heading
    height: 60vh

    &__text
      transform: translateY(100%)
</style>
