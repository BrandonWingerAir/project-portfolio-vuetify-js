<template>
    <v-row>
        <v-col cols="12" class="block-padding">
          <div class="block-1">
            <v-row>
              <v-col cols="12">
                <div class="block-section bg-color-1">
                  <v-icon color="#0091ea" x-large class="ml-3">
                    mdi-palette-swatch
                  </v-icon>
                  <h3 class="ml-3 mt-4">UI/UX</h3>
                  <ul class="text--lighten-1 ml-3 mt-5 mb-4">
                    <li>
                      Responsive websites, cross-device applications & PWA's
                    </li>
                    <li>
                      JavaScript animation, advanced calculators and interactive games
                    </li>
                  </ul>
                  <v-btn color="#0091ea" dark text @click="scroll('projects-scroll')">
                    more info
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>

                <div class="block-section bg-color-2">
                  <v-icon x-large class="ml-3" dark>
                    mdi-shopping
                  </v-icon>
                  <h3 class="white--text ml-3 mt-4">E-Commerce</h3>
                  <ul class="white--text text--lighten-2 ml-3 mt-5 mb-4">
                    <li>
                      WooCommerce (WordPress), PayPal & Stripe integration
                    </li>
                    <li>
                      Custom designs or theme additions and QA/improvement
                    </li>
                  </ul>
                  <v-btn dark text @click="scroll('projects-scroll')">
                    more info
                    <v-icon right>mdi-arrow-right</v-icon>
                  </v-btn>
                </div>

                <div class="block-section bg-color-1" id="about-scroll">
                  <v-icon color="#0091ea" x-large class="ml-3">
                    mdi-material-design
                  </v-icon>
                  <h3 class="ml-3 mt-4">Digital Production</h3>
                  <ul class="text--lighten-1 ml-3 mt-5 mb-4">
                    <li>
                      Documents & graphics (Logos, photograph editing etc.)
                    </li>
                    <li>
                      Design/AV software, engineering and multimedia branding
                    </li>
                  </ul>
                  <v-btn color="#0091ea" dark text @click="scroll('projects-scroll')">
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
                  <h3 class="mt-4">Years Experience</h3>
                </div>

                <div class="block-section-2 right-margin">
                  <v-row>
                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 block-margin block-padding bg-color-1">
                        <h1 class="blue--text">10+</h1>
                        <p>Satisfied Clients</p>
                      </div>
                    </v-col>

                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 sm-margin block-padding bg-color-1">
                        <h1 class="blue--text">15+</h1>
                        <p>Completed Projects</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>

                <div class="block-section-2">
                  <v-row>
                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 block-margin block-padding bg-color-1">
                        <h1 class="blue--text">30+</h1>
                        <p>Courses Completed</p>
                      </div>
                    </v-col>

                    <v-col cols="12" class="block-section-col">
                      <div class="block-section-2 block-padding bg-color-1">
                        <h1 class="blue--text">50+</h1>
                        <p id="projects-scroll">Tutorials Followed</p>
                      </div>
                    </v-col>
                  </v-row>
                </div>
              </v-col>
            </v-row>
          </div>
        </v-col>
    </v-row>
</template>

<script>
    export default {
      methods: {
          scroll(refName) {
              const element = document.getElementById(refName);
              element.scrollIntoView({ behavior: "smooth" });
          }
      }
    }
</script>

<style scoped>
.block-padding {
  padding: 8px 0;
}

.block-1 {
  width: 100%;
  height: 653px;

  background: linear-gradient(
    to right,
    #f5f5f5,
    #f5f5f5 50%,
    #fff 50%,
    #fff 50%
  );

  text-align: center;
  padding: 2rem 2rem;
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
  background-color: #e0e0e0;
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

h1.number {
  font-size: 50px;
  font-weight: bold;
}

.block-section-col {
  padding: 0 !important;
}

.block-margin {
  margin-bottom: 8px;
}

@media only screen and (max-width: 1408px) {
  .block-1 {
    height: 990px;
  }

  .block-section {
    margin-bottom: 8px;
  }
}

@media only screen and (max-width: 960px) {
  .block-1 {
    height: 1285px;
  }

  .block-section {
    margin-bottom: 10px;
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
  .block-section {
    width: 315px;
    margin: 5px auto;
  }
}

@media only screen and (max-width: 380px) {
  .block-1 {
    height: 1870px;
  }

  .block-section {
    width: 255px;
  }
}
</style>