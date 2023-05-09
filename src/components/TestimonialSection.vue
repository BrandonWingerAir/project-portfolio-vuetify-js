<template>
      <v-card class="mx-auto my-12 text-center" width="50%">
        <v-carousel hide-delimiters>
            <v-carousel-item
              v-for="(item,i) in items"
              :key="i"
            >
              <v-sheet
                height="100%"
                color="grey"
              >
                <v-row
                  class="fill-height"
                  align="center"
                  justify="center"
                >
                  <div>
                    <p>{{ item.review }}</p>
                    <h4>{{ item.client }}</h4>
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
            client: "Upwork client (Calculator - JavaScript/WordPress)",
            review: "Wonderful experience, thank you very much, fast, reliable and professional, I definitely recommend him to everyone, one of the best!"
          },
          {
            client: "",
            review: "2"
          }
        ],
      }
    },
  }
</script>