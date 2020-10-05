<template>
    <v-app>
        <v-main class="app-container">
            <v-row>
                <v-col cols="3">
                    <v-card
                            outlined
                            class="border-transparent mt-10 ml-12"
                            width="250"
                            height="50"
                    >
                        <v-row class="align-center">
                            <v-col cols="10">
                                <v-autocomplete
                                        dense
                                        solo
                                        flat
                                        label="Эксперт"
                                        class="border-transparent mt-n2"
                                ></v-autocomplete>
                            </v-col>
                            <v-img
                                    contain
                                    src="./images/Vector.png"
                                    height="20"
                                    class="ml-n7 mt-n7"
                            >
                            </v-img>
                        </v-row>
                    </v-card>
                    <card-scroll></card-scroll>
                </v-col>
                <users-info></users-info>
            </v-row>
        </v-main>
    </v-app>
</template>

<script>

    import CardScroll from "./components/card-scroll/CardScroll";
    import UsersInfo from "./components/users-info/UsersInfo";
    import './app.scss';

    export default {
        name: 'App',

        components: {CardScroll, UsersInfo},

        data: () => ({
        }),
    };
</script>
