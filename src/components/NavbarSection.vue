<template>
    <v-app-bar app color="#111111" dark flat class="px-8" max-width="100vw">
        <v-btn icon>
            <v-icon color="#039be5">fa-solid fa-globe</v-icon>
        </v-btn>
        <v-spacer class="xs-hide"></v-spacer>
        <v-btn text @click="scroll('home')" class="xxs-hide">Home</v-btn>
        <v-btn text @click="scroll('projects-scroll')">Projects</v-btn>
        <v-btn text @click="scroll('about-scroll')">About</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
    </v-app-bar>
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
@media only screen and (max-width: 600px) {
    .v-toolbar {
        padding-left: 4vw !important;
    }

    button {
        padding-left: 4vw !important;
        padding-right: 4vw !important;
    }

    .xs-hide {
        display: none;
    }

    
}

@media only screen and (max-width: 500px) {
    .v-toolbar {
        padding-left: 2vw !important;
    }

    button {
        padding-left: 3vw !important;
        padding-right: 3vw !important;
    }
}

@media only screen and (max-width: 400px) {
    .xxs-hide {
        display: none;
    }
}
</style>