<template>
    <v-app id="home" :style="{ background: $vuetify.theme.themes.dark.background }">
        <nav-bar />
        <v-container fluid>
            <v-row>
                <v-col cols="6">
                    <v-img src="1.png" contain max-height="500"></v-img>
                </v-col>
                <v-col cols="6">
                    <h5 class="red--text text--darken-4 top">Haii Aku Adam</h5>
                    <h1 class="white--text">Graphic Designer</h1>
                    <p class="grey--text">
                        Saya mahasiswa semester 4 di Universitas Brawijaya <br />
                        Fakultas Ilmu Komputer, program studi teknologi informasi. <br />
                        Saya memiliki ketertarikan dalam bidang desain grafis dan UI/UX Design<br />
                    </p>
                    <v-btn tile color="#A7121D" dark> about me </v-btn>
                </v-col>
                <v-col md="3" offset-md="3" id="project">
                    <h1 class="white--text">My Project Design</h1>
                </v-col>
                <v-col md="3" class="text-end">
                    <v-btn tile color="#A7121D" dark> View All </v-btn>
                </v-col>
                <v-col md="3" offset-md="3">
                    <v-card class="pa-2 py-12" outlined tile height="300px" color="#1E1E1E">
                        <v-img src="3.png" contain max-height=""></v-img>
                    </v-card>
                </v-col>
                <v-col md="3">
                    <v-card class="pa-2 py-12" outlined tile height="300px" color="#1E1E1E">
                        <v-img src="2.png" contain max-height=""></v-img>
                    </v-card>
                </v-col>
                <v-col md="3" offset-md="3">
                    <v-card class="pa-2 py-12" outlined tile height="250px" color="#1E1E1E">
                        <v-img src="4.png" contain max-height="170px"></v-img>
                    </v-card>
                </v-col>
                <v-col md="3">
                    <v-card class="pa-2 py-12" outlined tile height="250px" color="#1E1E1E">
                        <v-img src="5.png" contain max-height="170px"></v-img>
                    </v-card>
                </v-col>

                <v-col cols="12" class="padd topInverse">
                    <div class="second">
                        <div class="secondchild1" id="contact">
                            <h1 class="white--text">Hubungi saya</h1>
                            <p class="grey--text">
                                muhadamibrahim1873@gmail.com<br />
                                instagram.com/dammm_zx
                            </p>
                        </div>
                    </div>
                    <v-toolbar class="topTolbar" color="#111111" dark flat>
                        <div style="position: absolute; margin-left: auto; margin-right: auto; left: 0; right: 0; text-align: center">
                            <v-btn text>Home</v-btn>
                            <v-btn text>Project</v-btn>
                            <v-btn text>Contact</v-btn>
                        </div>
                    </v-toolbar>
                </v-col>
            </v-row>
        </v-container>
    </v-app>
</template>

<script>
import NavBar from "../components/NavBar.vue";

export default {
    name: "Home",
    data: () => ({
        icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
    }),
    components: {
        NavBar,
    },
};
</script>
<style scoped>
.top {
    margin-top: 180px;
}
.topInverse {
    margin-top: -250px;
}
.topTolbar {
    margin-top: 100px;
    text-align: center;
}
.second {
    width: 100%;
    height: 400px;
    background: #181818;
    text-align: center;
    padding: 2rem 2rem;
}
.secondchild1 {
    display: inline-block;
    background-color: #1e1e1e;
    padding: 2rem 1rem;
    vertical-align: middle;
    text-align: left;
    margin-top: 250px;
}
</style>
