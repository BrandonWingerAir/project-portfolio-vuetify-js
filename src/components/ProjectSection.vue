<template>
    <v-row>
        <v-col md="3" offset-md="3" offset-sm="1" order-md="1" order-sm="1" order="1">
            <h4 class="white--text">Featured Projects</h4>
            <p class="grey--text">Some of my recent work</p>
        </v-col>

        <v-col md="3" offset-md="1" class="text-end mr-offset" order-md="2" order-sm="2" order="2">
            <v-btn tile color="#0277bd" class="view-all-btn" dark href="https://github.com/BrandonWingerAir" target="_blank">Github</v-btn>
        </v-col>

        <!-- Project 1 Image-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="3" order-sm="3" order="3">
            <v-card href="https://www.indesigns.space/" target="_blank" class="px-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="indesigns-interior-decor.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <!-- Project 3 Image-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="7" order-sm="7" order="7">
            <v-card href="https://brandonwingerair.github.io/recipe-categories-api-js/" target="_blank" class="px-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="combined-rating-calculator.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <!-- Project 1 Info-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="5" order-sm="4" order="4">
            <v-btn color="white" dark text class="px-3 mr-1" href="https://www.indesigns.space/" target="_blank">
                inDesigns© Page (Branding & Vuetify)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="px-3" href="https://github.com/BrandonWingerAir/interior-decor-vuetify-js" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 3 Info-->
        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="9" order-sm="8" order="8">
            <v-btn color="white" dark text class="px-3 mr-1" href="https://brandonwingerair.github.io/recipe-categories-api-js/ " target="_blank">
                Multi-step Calculator (HTML/CSS, JS & PHP)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="px-3" href="https://github.com/BrandonWingerAir/recipe-categories-api-js" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 2 Image-->
        <v-col md="3" sm="10" offset-sm="1" order-md="4" order-sm="5" order="5" class="mr-offset">
            <v-card href="https://brandonwingerair.github.io/kanban-board-app-js/" target="_blank" class="px-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="kanban-web-app-js.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <!-- Project 4 Image-->
        <v-col md="3" sm="10" offset-sm="1" order-md="8" order-sm="9" order="9" class="mr-offset">
            <v-card href="https://brandonwingerair.github.io/web-project-cost-estimator/" target="_blank" class="px-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="client-cost-estimator.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <!-- Project 2 Info-->
        <v-col md="3" sm="10" offset-sm="1" order-md="6" order-sm="6" order="6" class="mr-offset">
            <v-btn color="white" dark text class="px-3 mr-1" href="https://brandonwingerair.github.io/kanban-board-app-js/" target="_blank">
                Kanban Board (HTML/CSS & JavaScript)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="px-3" href="https://github.com/BrandonWingerAir/kanban-board-app-js" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <!-- Project 4 Info-->
        <v-col md="3" sm="10" offset-sm="1" order-md="10" order-sm="10" order="10" class="mr-offset">
            <v-btn color="white" dark text class="px-3 mr-1" href="https://brandonwingerair.github.io/web-project-cost-estimator/" target="_blank">
                Cost & Time Estimator (Bulma + jQuery)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="px-3" href="hhttps://github.com/BrandonWingerAir/web-project-cost-estimator" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        
    }
</script>

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
</style>