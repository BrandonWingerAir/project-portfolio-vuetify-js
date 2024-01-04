<template>
    <v-footer dark padless>
        <v-card flat tile class="grey lighten-4 py-5 black--text px-5 text-center" width="100%">
            <v-row>
                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn icon @click="scroll('home')">
                            <v-icon color="#0091ea">fa-solid fa-globe</v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>

                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn 
                            v-for="icon in icons" 
                            :key="icon" 
                            class="mx-1 black--text" 
                            icon 
                            :href="icon.url"
                            target="_blank"
                        >
                            <v-icon size="24px">{{icon.image}}</v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>

                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn class="white--text" icon>
                            <v-icon color="#0091ea">mdi-brush-variant</v-icon>
                        </v-btn>
                        Brandon Winger-Air | 2023
                    </v-card-text>
                </v-col>
            </v-row>
        </v-card>
    </v-footer>
</template>

<script>
    export default {
        data: () => ({
            icons: [
                {
                    image: "mdi-linkedin",
                    url: "https://www.linkedin.com/in/bwingerair/"
                },
                {
                    image: "mdi-briefcase",
                    url: "https://www.freelancer.com/u/BWinger"
                },
                {
                    image: "mdi-github",
                    url: "https://github.com/BrandonWingerAir"
                }
            ]
        }),
        methods: {
            scroll(refName) {
                const element = document.getElementById(refName);
                element.scrollIntoView({ behavior: "smooth" });
            }
        }
    }
</script>