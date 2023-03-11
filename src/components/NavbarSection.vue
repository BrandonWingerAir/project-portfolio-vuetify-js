<template>
    <v-app-bar app color="#111111" dark flat class="px-8" max-width="100vw">
        <v-btn icon>
            <v-icon color="#039be5">fa-solid fa-globe</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')" class="xs-hide">Home</v-btn>
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
        padding-left: 20px !important;
        padding-right: 10px !important;
    }

}

@media only screen and (max-width: 480px) {
    .xs-hide {
        display: none;
    }
}

@media only screen and (max-width: 380px) {
    .v-btn {
        padding: 8px !important;
    }

    .v-toolbar {
        padding-left: 10px !important;
    }
}

@media only screen and (max-width: 325px) {
    .v-toolbar {
        padding-left: 0px !important;
        padding-right: 0px !important;
    }
}
</style>