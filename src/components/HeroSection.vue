<template>
    <v-row>
        <v-col sm="6">
            <v-img src="computer-tablet-and-smartphone.png" class="hero-img" max-height="500" contain></v-img>
        </v-col>
        <v-col sm="6" class="hero-block">
            <h5 class="light-blue--text text-darken-3 intro-text">Hello, I'm Brandon.</h5>
            <h1 class="white--text">Developer | Designer</h1>
            <p class="grey--text">
            ~ Enterprise Web & Mobile App Degree
            <br>
            ~ Freelance (InDesign/Photoshop, WordPress, HTML/CSS, JavaScript) 
            <br>
            ~ PHP, Linux, MySQL (Vue.js, Laravel, Tailwind etc.)
            </p>
            <v-btn tile color="a7121d" class="text-capitalize" dark href="https://www.upwork.com/freelancers/~01889fb0e8f4f710b7" target="_blank">Upwork</v-btn>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .intro-text {
        margin-top: 175px;
        font-size: 19px;
    }

    @media only screen and (max-width: 960px) {
        .hero-block {
            margin-bottom: 18px;
        }

        .intro-text {
            margin-top: 0;
        }
    }

    @media only screen and (max-width: 600px) {
        .hero-img {
            margin-top: -68px;
        }

        .hero-block {
            margin-bottom: 35px;
            padding: 0 50px;
        }

        .intro-text {
            margin-top: -60px;
        }
    }

    @media only screen and (max-width: 380px) {
        .hero-block {
            padding: 0 40px;
        }
    }

    @media only screen and (max-width: 325px) {
        .hero-block {
            padding: 0 25px;
        }
    }
</style>