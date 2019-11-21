<template>
  <v-app>
    <appMenu />
    <v-content>
      <nuxt />
    </v-content>
  </v-app>
</template>

<script>
import AppMenu from '~/components/index/AppMenu'

export default {
  components: {
    AppMenu
  }
}
</script>
