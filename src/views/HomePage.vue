<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.light.background }">
    <HeaderSection/>

    <v-container fluid>
      <HeroSection/>
      <AboutSection/>
      <ProjectSection/>
      <TestimonialSection/>
      <ContactSection/>
    </v-container>

    <FooterSection/>
  </v-app>
</template>

<script>
  import HeaderSection from '../components/site/HeaderSection'
  import HeroSection from '../components/HeroSection'
  import AboutSection from '../components/AboutSection'
  import ProjectSection from '../components/ProjectSection'
  import TestimonialSection from '../components/TestimonialSection'
  import ContactSection from '../components/ContactSection'
  import FooterSection from '../components/site/FooterSection'

  export default {
    name: 'HomePage',

    components: {
      HeaderSection,
      HeroSection,
      AboutSection,
      ProjectSection,
      TestimonialSection,
      ContactSection,
      FooterSection
    },
  }
</script>