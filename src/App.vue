<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background }">
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style>
.block-2 {
  width: 100%;
  background-color: #eee;
  text-align: center;
  padding: 2rem 2rem 3rem;
}

.block-3 {
    width: 75%;
}

@media only screen and (max-width: 600px) {
  .block-3 h4 {
      font-size: 23px !important;
  }

  .block-3 hr {
      width: 235px;
  }
}
</style>