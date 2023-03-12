<template>
    <v-row>
        <v-col cols="12" class="pa-0 topInverse" order-md="11" order-sm="11" order="11">
            <div class="block-2">
                <div class="block-2_section-1" id="contact">
                    <v-row>
                    <v-col cols="12" sm="7">
                        <h1 class="white--text contact-text">
                        Let's work,
                        <br> connect:
                        </h1>
                        <p class="grey--text">
                        brandon.air.web@gmail.com
                        <br>
                        </p>
                    </v-col>
                    <v-col cols="12" sm="5">
                        <v-btn tile color="#0277bd" dark class="mt-sm-16 mt-n5">
                        <a href="mailto:brandon.air.web@gmail.com" class="white--text text-decoration-none">Contact Me</a>
                        </v-btn>
                    </v-col>
                    </v-row>
                </div>
            </div>

            <!-- Footer Menu: Requires hiding top navbar after scrolling -->
            <!-- <v-toolbar class="bottomNavbar" color="#111111" dark flat>
            <div style="position: absolute; margin-left: auto; margin-right: auto; left: 0; right: 0; text-align: center;">
                <v-btn text>Home</v-btn>
                <v-btn text>Projects</v-btn>
                <v-btn text>About</v-btn>
                <v-btn text>Contact</v-btn>
            </div>
            </v-toolbar> -->
        </v-col>
    </v-row>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.topInverse {
  margin-top: -250px;
}

.block-2 {
    width: 100%;
    height: 545px;
    background: #181818;
    text-align: center;
    padding: 2rem 2rem;
}

.block-2_section-1 {
    width: 675px;
    display: inline-block;
    background-color: #1e1e1e;
    padding: 2rem 2.5rem;
    vertical-align: middle;
    text-align: left;
    margin-top: 250px;
}

/* .bottomNavbar {
  margin-top: 100px;
  text-align: center;
} */

@media only screen and (max-width: 960px) {
    .block-2_section-1 {
        width: 535px;
    }

    .contact-text {
        font-size: 28px;
    }
}

@media only screen and (max-width: 600px) {
    .block-2 {
        height: 575px;
    }

    .block-2_section-1 {
        width: 320px;
    }
}

@media only screen and (max-width: 380px) {
    .block-2_section-1 {
        width: 260px;
        padding: 20px 16px;
    }
}
</style>