<template>
  <v-app id="home" :style="{ background: $vuetify.theme.themes.dark.background }">
    <NavbarSection/>
    <v-container fluid>
      <v-row>
        <v-col sm="6">
          <v-img src="computer-tablet-and-smartphone.png" class="hero-img" max-height="500" contain></v-img>
        </v-col>
        <v-col sm="6" class="hero-block">
          <h5 class="light-blue--text text-darken-3 intro-text">Hello, I'm Brandon.</h5>
          <h1 class="white--text">Developer | Designer</h1>
          <p class="grey--text">
            ~ Enterprise Web & Mobile App Degree
            <br>
            ~ Freelance (InDesign/Photoshop, WordPress, HTML/CSS, JavaScript) 
            <br>
            ~ PHP, Linux, MySQL (Vue.js, Laravel, Tailwind etc.)
          </p>
          <v-btn tile color="a7121d" dark>cv/résumé</v-btn>
        </v-col>

        <v-col cols="12" class="padding">
          <div class="block-1">
            <v-row>
              <v-col cols="12">
                <div class="block-section bg-color-1">
                  <v-icon color="#039be5" x-large class="ml-3">
                    mdi-palette-swatch
                  </v-icon>
                  <h3 class="white--text ml-3 mt-4">UI/UX</h3>
                  <p class="grey--text text--lighten-1 ml-3 mt-6">
                    ● Responsive websites, cross-device applications & PWA's
                    <br>
                    ● JavaScript animation, advanced calculator and games
                  </p>
                  <v-btn color="#03a9f4" dark text>
                    more info
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>

                <div class="block-section bg-color-2">
                  <v-icon x-large class="ml-3" dark>
                    mdi-shopping
                  </v-icon>
                  <h3 class="white--text ml03 mt-4">E-Commerce</h3>
                  <p class="grey--text text--lighten-2 ml-3 mt-6">
                    ● WooCommerce (WordPress), PayPal & Stripe integration
                    <br>
                    ● Custom designs or theme additions and QA/improvement
                  </p>
                  <v-btn dark text>
                    more info
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>

                <div class="block-section bg-color-1" id="about-scroll">
                  <v-icon color="#039be5" x-large class="ml-3">
                    mdi-material-design
                  </v-icon>
                  <h3 class="white--text ml-3 mt-4">Digital Production</h3>
                  <p class="grey--text text--lighten-1 ml-3 mt-6">
                    ● Documents & graphics (Logos, photograph editing etc.)
                    <br>
                    ● Design/AV software, engineering and multimedia branding
                  </p>
                  <v-btn color="#03a9f4" dark text>
                    more info
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>
              </v-col>

              <v-col cols="12" class="mt-md-10">
                <div class="block-section-1">
                  <h1 class="blue--text text-darken-4 mt-4 number">
                    8
                  </h1>
                  <h3 class="white--text mt-4">Years Experience</h3>
                </div>

                <div class="block-section-2 right-margin">
                  <v-row>
                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 button-margin padding bg-color-1">
                        <h1 class="light-blue--text">10+</h1>
                        <p class="grey--text">Satisfied Clients</p>
                      </div>
                    </v-col>

                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 sm-margin padding bg-color-1">
                        <h1 class="light-blue--text">15+</h1>
                        <p class="grey--text">Completed Projects</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>

                <div class="block-section-2">
                  <v-row>
                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 button-margin padding bg-color-1">
                        <h1 class="light-blue--text">30+</h1>
                        <p class="grey--text">Courses Completed</p>
                      </div>
                    </v-col>

                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 padding bg-color-1">
                        <h1 class="light-blue--text">50+</h1>
                        <p class="grey--text" id="projects-scroll">Tutorials Followed</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>

        <v-col md="3" offset-md="3" offset-sm="1" order-md="1" order-sm="1" order="1">
          <h4 class="white--text">Featured Projects</h4>
          <p class="grey--text">Some of my recent work</p>
        </v-col>

        <v-col md="3" offset-md="1" class="text-end" order-md="2" order-sm="2" order="2">
          <v-btn tile color="#0277bd" class="view-all-btn" dark>Coming Soon</v-btn>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="3" order-sm="3" order="3">
          <v-card class="pa-2 py-12" outlined tile color="#1e1e1e">
            <v-img src="coding.jpg" class="project-img" contain></v-img>
          </v-card>
        </v-col>
        
        <v-col md="3" sm="10" offset-sm="1" order-md="4" order-sm="5" order="5">
          <v-card class="pa-2 py-12" outlined tile color="#1e1e1e">
            <v-img src="coding.jpg" class="project-img" contain></v-img>
          </v-card>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="5" order-sm="4" order="4">
          <v-btn color="white" dark text class="ml-n4">
            Project 1
          </v-btn>
          <v-btn color="#03a9f4" dark text class="ml-n4">
            Details
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col md="3" sm="10" offset-sm="1" order-md="6" order-sm="6" order="6">
          <v-btn color="white" dark text class="ml-n4">
            Project 2
          </v-btn>
          <v-btn color="#03a9f4" dark text class="ml-n4">
            Details
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="7" order-sm="7" order="7">
          <v-card class="pa-2 py-12" outlined tile color="#1e1e1e">
            <v-img src="coding.jpg" class="project-img" contain></v-img>
          </v-card>
        </v-col>
        
        <v-col md="3" sm="10" offset-sm="1" order-md="8" order-sm="9" order="9">
          <v-card class="pa-2 py-12" outlined tile color="#1e1e1e">
            <v-img src="coding.jpg" class="project-img" contain></v-img>
          </v-card>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="9" order-sm="8" order="8">
          <v-btn color="white" dark text class="ml-n4">
            Project 3
          </v-btn>
          <v-btn color="#03a9f4" dark text class="ml-n4">
            Details
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col md="3" sm="10" offset-sm="1" order-md="10" order-sm="10" order="10">
          <v-btn color="white" dark text class="ml-n4">
            Project 4
          </v-btn>
          <v-btn color="#03a9f4" dark text class="ml-n4">
            Details
            <v-icon right>mdi-arrow-right</v-icon>
          </v-btn>
        </v-col>

        <v-col cols="12" class="padding topInverse" order-md="11" order-sm="11" order="11">
          <div class="block-2">
            <div class="block-2_section-1" id="contact">
              <v-row>
                <v-col cols="12" sm="7">
                  <h1 class="white--text contact-text">
                    Let's work,
                    <br> connect:
                  </h1>
                  <p class="grey--text">
                    brandon.air.web@gmail.com
                    <br>
                  </p>
                </v-col>
                <v-col cols="12" sm="5">
                  <v-btn tile color="#0277bd" dark class="mt-sm-16 mt-n5">
                    <a href="mailto:brandon.air.web@gmail.com" class="white--text text-decoration-none">Contact Me</a>
                  </v-btn>
                </v-col>
              </v-row>
            </div>
          </div>

          <!-- <v-toolbar class="topToolbar" color="#111111" dark flat>
            <div style="position: absolute; margin-left: auto; margin-right: auto; left: 0; right: 0; text-align: center;">
              <v-btn text>Home</v-btn>
              <v-btn text>Projects</v-btn>
              <v-btn text>About</v-btn>
              <v-btn text>Contact</v-btn>
            </div>
          </v-toolbar> -->
        </v-col>
      </v-row>
    </v-container>

    <FooterSection/>
  </v-app>
</template>

<script>
  import NavbarSection from '../components/NavbarSection'
  import FooterSection from '../components/FooterSection'

  export default {
    name: 'HomePage',

    components: {
      NavbarSection,
      FooterSection
    },
  }
</script>

<style scoped>
.intro-text {
  margin-top: 175px;
  font-size: 19px;
}

.topInverse {
  margin-top: -250px;
}

.topToolbar {
  margin-top: 100px;
  text-align: center;
}

.block-1 {
  width: 100%;
  height: 775px;

  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%
  );

  text-align: center;
  padding: 2rem 2rem;
}

.block-2 {
  width: 100%;
  height: 545px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}

.block-2_section-1 {
  width: 675px;
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 2.5rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 250px;
}

.block-section {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
  width: 440px;
}

.bg-color-1 {
  background-color: #1e1e1e;
}

.bg-color-2 {
  background-color: #0277bd;
}

.block-section-1 {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  margin-right: 5px;
  width: 240px;
}

.block-section-2 {
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

.col-12.block-section-col {
  padding: 0 !important;
}

h1.number {
  font-size: 50px;
  font-weight: bold;
}

.project-img {
  height: 250px;
}

@media only screen and (max-width: 1408px) {
  .block-1 {
    height: 990px;
  }

  .block-section {
    margin-bottom: 8px;
  }

  .project-img {
    height: 150px;
  }
}

@media only screen and (max-width: 960px) {
  .hero-block {
    margin-bottom: 18px;
  }

  .intro-text {
    margin-top: 0;
  }

  .block-1 {
    height: 1285px;
  }

  .block-section {
    margin-bottom: 10px;
  }

  .view-all-btn {
    right: 19%;
  }

  .project-img {
    height: 270px;
  }

  .block-2_section-1 {
    width: 535px;
  }

  .contact-text {
    font-size: 28px;
  }
}

@media only screen and (max-width: 806px) {
  .block-1 {
    height: 1720px;
  }

  .block-section-2 {
    display: block;
    margin: 5px auto;
  }

  .sm-margin {
    margin-bottom: 12px;
  }
}

@media only screen and (max-width: 600px) {
  .hero-img {
    margin-top: -68px;
  }

  .hero-block {
    margin-bottom: 35px;
    padding: 0 50px;
  }

  .intro-text {
    margin-top: -60px;
  }

  .block-section {
    width: 315px;
    margin: 5px auto;
  }

  .view-all-btn {
    right: 0;
  }

  .block-2 {
    height: 575px;
  }

  .block-2_section-1 {
    width: 320px;
  }
}

@media only screen and (max-width: 380px) {
  .hero-block {
    padding: 0 40px;
  }

  .block-1 {
    height: 1870px;
  }

  .block-section {
    width: 255px;
  }

  .block-2_section-1 {
    width: 260px;
    padding: 20px 16px;
  }
}

@media only screen and (max-width: 325px) {
  .hero-block {
    padding: 0 25px;
  }
}
</style>