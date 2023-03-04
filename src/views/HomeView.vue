<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <NavbarView/>
  </v-app>
</template>

<script>
  import NavbarView from '../components/NavbarView'

  export default {
    name: 'HomeView',

    components: {
      NavbarView,
    },
  }
</script>
