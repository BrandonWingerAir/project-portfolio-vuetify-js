<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.dark.background }">
    <NavbarSection/>

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
  import NavbarSection from '../components/NavbarSection'
  import HeroSection from '../components/HeroSection'
  import AboutSection from '../components/AboutSection'
  import ProjectSection from '../components/ProjectSection'
  import TestimonialSection from '../components/TestimonialSection'
  import ContactSection from '../components/ContactSection'
  import FooterSection from '../components/FooterSection'

  export default {
    name: 'HomePage',

    components: {
      NavbarSection,
      HeroSection,
      AboutSection,
      ProjectSection,
      TestimonialSection,
      ContactSection,
      FooterSection
    },
  }
</script>