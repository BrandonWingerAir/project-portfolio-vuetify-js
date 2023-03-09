<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
        <v-btn icon>
            <v-icon color="#039be5">fa-solid fa-globe</v-icon>
        </v-btn>
        <v-spacer class="xs-hide"></v-spacer>
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
        padding-left: 3% !important;
    }

    button {
        padding-left: 2% !important;
        padding-right: 2% !important;
    }

    .xs-hide {
        display: none;
    }
}

</style>