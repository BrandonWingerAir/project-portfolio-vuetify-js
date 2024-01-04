<template>
    <v-app-bar app dark flat class="grey lighten-4 px-8" max-width="100vw">
        <v-btn icon @click="scroll('home')">
            <v-icon color="#0091ea">fa-solid fa-globe</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('home')" class="xs-hide black--text">
            Home
        </v-btn>
        <v-btn text @click="scroll('projects-scroll')" class="pl-0 pr-2 px-sm-2 px-md-4 black--text">
            Portfolio
        </v-btn>
        <v-btn text href="https://github.com/BrandonWingerAir" target="_blank" class="px-0 px-sm-2 px-md-4 black--text">
            Github
        </v-btn>
        <v-btn text @click="scroll('about-scroll')" class="pl-0 pr-2 px-sm-2 px-md-4 black--text">
            About
        </v-btn>
        <v-btn text @click="scroll('contact')" class="px-0 px-sm-2 px-md-4 black--text">
            Contact
        </v-btn>
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
.v-toolbar {
    padding-right: 10px !important;
}

@media only screen and (max-width: 600px) {
    .v-btn {
        font-size: 12px;
    }

    .v-toolbar {
        padding-right: 0 !important;
    }
}

@media only screen and (max-width: 600px) {
    .v-toolbar {
        padding-left: 20px !important;
    }
}

@media only screen and (max-width: 480px) {
    .xs-hide {
        display: none;
    }
}

@media only screen and (max-width: 380px) {
    .v-btn {
        font-size: 11px;
    }

    .v-toolbar {
        padding-left: 10px !important;
    }
}

@media only screen and (max-width: 325px) {
    .v-toolbar {
        padding-left: 0px !important;
    }
}
</style>