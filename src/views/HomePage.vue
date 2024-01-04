<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.light.background }">
    <SiteHeader/>

    <v-container fluid>
      <HeroSection/>
      <AboutSection/>
      <ProjectSection/>
      <TestimonialSection/>
      <ContactSection/>
      <CertificateSection/>
    </v-container>

    <SiteFooter/>
  </v-app>
</template>

<script>
  import SiteHeader from '../components/SiteHeader';
  import HeroSection from '../components/sections/HeroSection';
  import AboutSection from '../components/sections/AboutSection';
  import ProjectSection from '../components/sections/ProjectSection';
  import TestimonialSection from '../components/sections/TestimonialSection';
  import ContactSection from '../components/sections/ContactSection';
  import CertificateSection from '../components/sections/CertificateSection';
  import SiteFooter from '../components/SiteFooter';

  export default {
    name: 'HomePage',

    components: {
      SiteHeader,
      HeroSection,
      AboutSection,
      ProjectSection,
      TestimonialSection,
      ContactSection,
      CertificateSection,
      SiteFooter
    },
  }
</script>