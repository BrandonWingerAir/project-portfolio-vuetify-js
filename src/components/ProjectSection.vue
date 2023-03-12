<template>
    <v-row>
        <v-col md="3" offset-md="3" offset-sm="1" order-md="1" order-sm="1" order="1">
            <h4 class="white--text">Featured Projects</h4>
            <p class="grey--text">Some of my recent work</p>
        </v-col>

        <v-col md="3" offset-md="1" class="text-end mr-offset" order-md="2" order-sm="2" order="2">
            <v-btn tile color="#0277bd" class="view-all-btn" dark href="https://github.com/BrandonWingerAir" target="_blank">Github</v-btn>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="3" order-sm="3" order="3">
            <v-card class="pa-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="recipes-api-app-js.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <v-col md="3" sm="10" offset-sm="1" order-md="4" order-sm="5" order="5" class="mr-offset">
            <v-card class="pa-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="list-app-vue-js.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="5" order-sm="4" order="4">
            <v-btn color="white" dark text class="ml-n4" href="https://brandonwingerair.github.io/recipe-categories-api-js/" target="_blank">
                Recipes API Website (JS)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="ml-n4" href="https://github.com/BrandonWingerAir/recipe-categories-api-js" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <v-col md="3" sm="10" offset-sm="1" order-md="6" order-sm="6" order="6" class="mr-offset">
            <v-btn color="white" dark text class="ml-n4" href="https://brandonwingerair.github.io/todo-app-vue-js/ " target="_blank">
                List Web App (Vue 3)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="ml-n4" href="https://github.com/BrandonWingerAir/todo-app-vue-js " target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="7" order-sm="7" order="7">
            <v-card class="pa-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="kanban-web-app-js.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>
        
        <v-col md="3" sm="10" offset-sm="1" order-md="8" order-sm="9" order="9" class="mr-offset">
            <v-card class="pa-6 py-12" outlined tile color="#1e1e1e">
                <v-img src="platformer-game-phaser-ts.png" class="project-img" contain></v-img>
            </v-card>
        </v-col>

        <v-col md="3" offset-md="3" sm="10" offset-sm="1" order-md="9" order-sm="8" order="8">
            <v-btn color="white" dark text class="ml-n4" href="https://brandonwingerair.github.io/kanban-board-app-js/" target="_blank">
                Kanban Web App (JS)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="ml-n4" href="https://github.com/BrandonWingerAir/kanban-board-app-js" target="_blank">
                Code
                <v-icon right>mdi-arrow-right</v-icon>
            </v-btn>
        </v-col>

        <v-col md="3" sm="10" offset-sm="1" order-md="10" order-sm="10" order="10" class="mr-offset">
            <v-btn color="white" dark text class="ml-n4" href="https://brandonwingerair.github.io/platformer-game-phaser-ts/" target="_blank">
                Platform Game (Phaser/TypeScript)
            </v-btn>
            <v-btn color="#03a9f4" dark text class="ml-n4" href="https://github.com/BrandonWingerAir/platformer-game-phaser-ts" target="_blank">
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