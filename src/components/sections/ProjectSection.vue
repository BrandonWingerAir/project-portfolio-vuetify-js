<template>
    <v-row>
        <v-col md="3" offset-md="3" offset-sm="1" order-md="1" order-sm="1" order="1">
            <h4>Featured Projects</h4>
            <p class="grey--text">Some of my recent work</p>
        </v-col>

        <v-col md="3" offset-md="1" class="text-end mr-offset" order-md="2" order-sm="2" order="2">
            <v-btn tile color="#0277bd" class="view-all-btn" dark href="https://www.upwork.com/freelancers/~01889fb0e8f4f710b7" target="_blank">Upwork Profile</v-btn>
        </v-col>

        <!-- Project 1 Image-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="3" order-sm="3" order="3">
            <v-card href="https://philipcomanphotography.com/" target="_blank" class="px-6 py-12" outlined tile color="#eeeeee">
                <v-img src="philip-coman-photography-site.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <!-- Project 3 Image-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="7" order-sm="7" order="7">
            <v-card href="https://brandonwingerair.github.io/matrix-multi-calculator-js/" target="_blank" class="px-6 py-12" outlined tile color="#eeeeee">
                <v-img src="combined-rating-calculator.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <!-- Project 1 Info-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="5" order-sm="4" order="4">
            <v-btn color="black" dark text class="px-3 mr-1" href="https://philipcomanphotography.com/" target="_blank">
                Photographer Site (HTML/CSS & Vuetify)
            </v-btn>
            <v-btn color="#0091ea" dark text class="px-3" href="https://github.com/BrandonWingerAir/interior-decor-vuetify-js" target="_blank">
                View Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 3 Info-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="9" order-sm="8" order="8">
            <v-btn color="black" dark text class="px-3 mr-1" href="https://brandonwingerair.github.io/matrix-multi-calculator-js/ " target="_blank">
                Matrix Calculator (JS, WordPress & PHP)
            </v-btn>
            <v-btn color="#0091ea" dark text class="px-3" href="https://github.com/BrandonWingerAir/matrix-multi-calculator-js" target="_blank">
                View Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 2 Image-->
        <v-col md="3" sm="10" offset-sm="1" order-md="4" order-sm="5" order="5" class="mr-offset">
            <v-card href="https://brandonwinger-air.com/web-project-calculator/" target="_blank" class="px-6 py-12" outlined tile color="#eeeeee">
                <v-img src="client-cost-estimator.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <!-- Project 4 Image-->
        <v-col md="3" sm="10" offset-sm="1" order-md="8" order-sm="9" order="9" class="mr-offset">
            <v-card href="https://blog.brandonwinger-air.com/" target="_blank" class="px-6 py-12" outlined tile color="#eeeeee">
                <v-img src="responsive-thumbnail-blog-portfolio.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <!-- Project 2 Info-->
        <v-col md="3" sm="10" offset-sm="1" order-md="6" order-sm="6" order="6" class="mr-offset">
            <v-btn color="black" dark text class="px-3 mr-1" href="https://brandonwinger-air.com/web-project-calculator/" target="_blank">
                Cost + Time Estimator (Bulma & jQuery)
            </v-btn>
            <v-btn color="#0091ea" dark text class="px-3" href="https://github.com/BrandonWingerAir/web-project-cost-estimator" target="_blank">
                View Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 4 Info-->
        <v-col md="3" sm="10" offset-sm="1" order-md="10" order-sm="10" order="10" class="mr-offset">
            <v-btn color="black" dark text class="px-3 mr-1" href="https://blog.brandonwinger-air.com/" target="_blank">
                Blog Website (Nuxt, Tailwind & GraphQL)
            </v-btn>
            <v-btn color="#0091ea" dark text class="px-3" href="https://github.com/BrandonWingerAir/portfolio-nuxt-tailwind-graphql" target="_blank">
                View Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>
    </v-row>
</template>

<style scoped>
.mr-offset {
    position: relative;
    right: 5%;
}

.project-img {
  height: 250px;
}

@media only screen and (max-width: 1408px) {
  .project-img {
    height: 150px;
  }
}

@media only screen and (max-width: 960px) {
    .mr-offset {
        right: 0;
    }

    .view-all-btn {
        right: 19%;
    }

    .project-img {
        height: 270px;
    }
}

@media only screen and (max-width: 600px) {
  .view-all-btn {
    right: 0;
  }
}

@media only screen and (max-width: 438px) {
  .v-btn {
    font-size: 12px;
  }
}
</style>