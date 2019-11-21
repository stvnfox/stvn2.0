<template>
  <v-app-bar color="#fafafa" flat app absolute>
    <v-dialog
      v-model="dialog"
      fullscreen
      transition="slide-y-transition"
    >
      <template v-slot:activator="{ on }">
        <v-app-bar-nav-icon>
          <v-icon v-on="on">
            mdi-menu
          </v-icon>
        </v-app-bar-nav-icon>
      </template>
      <v-container fill-height fluid class="grey">
        <v-btn @click="dialog = false">
          <v-icon>mdi-close</v-icon>
        </v-btn>
      </v-container>
    </v-dialog>
    <v-toolbar-title class="text-right grey--text" style="width: 100%">
      SV
    </v-toolbar-title>
  </v-app-bar>
</template>

<script>
export default {
  name: 'AppMenu',
  data () {
    return {
      dialog: false
    }
  }
}
</script>

<style lang="sass" scoped>

</style>
