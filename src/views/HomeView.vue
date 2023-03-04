<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.dark.background }">
    <NavbarView/>
    <v-container fluid>
      <v-row>
        <v-col cols="6">
          <v-img src="computer-tablet-and-smartphone.png" contain max-height="500"></v-img>
        </v-col>
        <v-col cols="6">
          <h5 class="light-blue--text text-darken-4 top">Hello, I'm Brandon</h5>
          <h1 class="white--text">Designer | Developer</h1>
          <p class="grey--text">
            ~ Enterprise Web & Mobile App Development Degree
            <br>
            ~ Freelance (InDesign/Photoshop, WordPress, HTML/CSS, JavaScript) 
            <br>
            ~ Vue.js + Laravel (Nuxt, Vuetify, Tailwind etc.)
          </p>
          <v-btn tile color="a7121d" dark>cv/résumé</v-btn>
        </v-col>
      </v-row>
    </v-container>
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

<style scoped>
.top {
  margin-top: 180px;
}

.topInverse {
  margin-top: -250px;
}

.topTolbar {
  margin-top: 100px;
  text-align: center;
}

.block-1 {
  width: 100%;
  height: 610px;

  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%,
  );

  text-align: center;
  padding: 2rem 2rem;
}

.block-2 {
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}

.block-2_child-1 {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}

.block-child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}

.bg-color-1 {
  background-color: #1e1e1e;
}

.bg-color-2 {
  background-color: #ce1d2a;
}

.block-child-1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}

.block-child-2 {
  display: inline-block;
  width: 245px;
  vertical-align: middle;
}

.right-margin {
  margin-right: 8px;
}

.button-margin {
  margin-bottom: 8px;
}

.padding {
  padding: 8px 0;
}

.col-12.col-padding {
  padding: 12px 0 !important;
}

.col-12.child-col {
  padding: 0 !important;
}

h1.number {
  font-size: 50px;
  font-weight: bold;
}
</style>
