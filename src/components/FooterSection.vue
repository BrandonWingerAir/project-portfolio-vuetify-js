<template>
    <v-footer dark padless>
        <v-card flat tile class="black white--text py-5 px-5 text-center" width="100%">
            <v-row>
                <v-col cols="12" sm="4">
                    <v-card-text class="white--text pt-2">
                        <v-btn icon @click="scroll('home')">
                            <v-icon color="#039be5">fa-solid fa-globe</v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>

                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn 
                            v-for="icon in icons" 
                            :key="icon" 
                            class="mx-1 white--text" 
                            icon 
                            href="https://www.linkedin.com/in/bwingerair/" 
                            target="_blank"
                        >
                            <v-icon size="24px">{{icon}}</v-icon>
                        </v-btn>
                    </v-card-text>
                </v-col>

                <v-col cols="12" sm="4">
                    <v-card-text class="pt-2">
                        <v-btn class="white--text" icon>
                            <v-icon color="#039be5">mdi-brush-variant</v-icon>
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
                "mdi-linkedin"
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