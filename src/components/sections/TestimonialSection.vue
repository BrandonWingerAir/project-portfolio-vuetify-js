<template>
  <v-card id="testimonials-carousel" class="mx-auto my-12 text-center pt-4 bg-color-3" width="75%">
        <h2 class="mb-4 grey--text text--darken-4">Testimonials</h2>
        <hr>
        <v-carousel hide-delimiters>
            <v-carousel-item
              v-for="(item,i) in items"
              :key="i"
            >
              <v-sheet
                height="100%"
                class="bg-color-4"
              >
                <v-row
                  class="fill-height text--lighten-2"
                  align="center"
                  justify="center"
                >
                  <div class="review-container">
                    <p class="text--lighten-3">"{{ item.review }}"</p>
                    <h4>{{ item.client }}</h4>
                    <h5 class="mb-6">Project: {{ item.project }}</h5>
                    <v-btn :href="item.link" color="#e0e0e0">View Rating</v-btn>
                  </div>
                </v-row>
              </v-sheet>
            </v-carousel-item>
          </v-carousel>
        </v-card>
          
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            client: "Upwork.com client",
            review: "Wonderful experience, thank you very much, fast, reliable and professional, I definitely recommend him to everyone, one of the best!",
            project: "Calculator Plugin (JavaScript/WordPress)",
            link: "https://www.upwork.com/freelancers/~01889fb0e8f4f710b7"
          },
          {
            client: "Jeffrey S. @CityPopper - Freelancer.com",
            review: "No complaints.",
            project: "Site Feature (AliPay/Stripe & WordPress)",
            link: "https://www.freelancer.com/u/BWinger"
          },
          {
            client: "Katherine M. @kmyers1 - Freelancer.com",
            review: "Excellent communication! Will hire again!",
            project: "Site Feature (UserPro plugin for WordPress)",
            link: "https://www.freelancer.com/u/BWinger"
          },
          {
            client: "Love L. @Hopedove - Freelancer.com",
            review: "Very responsive work attitude.",
            project: "English Writing",
            link: "https://www.freelancer.com/u/BWinger"
          },
          {
            client: "Benjamin R. @dfservice - Freelancer.com",
            review: "cooperative Freelancer, nice to work with him.",
            project: "Site Feature (WooCommerce/Wordpress & Stripe)",
            link: "https://www.freelancer.com/u/BWinger"
          }
        ],
      }
    },
  }
</script>

<style scoped>
#testimonials-carousel {
  max-width: 800px;
  height: 558px;
  border: 2px solid #212121;
  border-radius: 0;
}

.bg-color-3 {
  background: #e0e0e0;
}

h2 {
  font-size: 26px;
}

hr {
  border-color: #212121;
}

.bg-color-4 {
  background-color: #fff;
  border-bottom: 2px solid #212121;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}

.review-container {
  padding: 0 75px;
}

.v-icon {
  padding: 20px !important;
}
</style>