<template>
  <v-container id='Mobile'>
        <v-card class="mx-auto">
          <v-row align="center" justify="center" dense>
            <v-spacer></v-spacer>
              <v-card flat tile :width="largueurImageDesktop" >
                  <v-img src="../../public/images/pic05.jpg" tile width="100%"></v-img>
              </v-card>
              <v-spacer></v-spacer>
              <v-spacer></v-spacer>
              <v-card flat tile class="mx-auto" :width="largueurTexteDesktop" >
                <br><br>
                <v-card-title>
                  <h2 class="subheading font-weight-bold mb-2">Mobile&nbsp;</h2>
                  <v-icon color="black">mdi-android</v-icon>
                </v-card-title>
                <v-card color="blue lighten-5">
                <v-card-title>
                  <h3 class="subheading font-weight-bold mb-2">Projet de groupe nommé 'plantGO' (septembre 2020-avril 2021)</h3>
                </v-card-title>
                </v-card>
                <v-row class="text-center">
                  <v-col class="mb-5" cols="12">
                    <v-card flat tile class="mx-auto">
                      <v-card-text style="font-size: 1.3em;line-height: 1.7em">
                        <p class="font-weight-regular" align="justify">
                          <b><i>Contexte</i></b> : Application mobile ludique Android qui vise à apporter des connaissances encyclopédiques par la collection de cartes de plantes,
                          à la manière d’un “herbier virtuel”. Une carte Google Maps indique une zone de recherche localisant les plantes à photographier. Le joueur profite
                          de pauses récréatives via l’obtention de cosmétiques afin de personnaliser son avatar ainsi que de deux mini-jeux de plateforme.
                          <br><br>
                            <b><i>Mon rôle</i></b> : Chef de projet.
                          <br><br>
                            <b><i>Mes tâches</i></b> :
                            <ul>
                              <li><i>Rédaction</i> : Organisation du plan des parties, écriture et relectures.
                              </li>
                              <li><i>Gestion</i> : Assignation des tâches, tenue des délais, gestion du projet via un Trello.</li>
                              <li><i>Programmation</i> : Développement des mini-jeux et intégration des maquettes.</li>
                            </ul>
                          <br>
                            <b><i>Rôle des autres membres du groupe</i></b> : Design UI / UX. Implémentation APIs.
                          <br><br>
                            <b><i>Technologies</i></b> :
                            <ul>
                              <li><i>Front-end Dev</i> : Android Studio (Java) avec le framework libGDX pour l'aspect jeu-vidéo.
                              </li>
                              <li><i>Front-end Design</i> : Design maquettes avec Figma. Level-Design des mini-jeux avec 'Tiled Map Editor' et import des sprites avec 'TexturePackerGUI'.</li>
                              <li><i>APIs</i> : Identification espèces botaniques à partir de photographies (pl@ntNet). Extraction données encyclopédiques (Trefle). Carte avec géolocalisation GPS (Google Maps).</li>
                            </ul>
                          <br><br>
                        </p>
                      </v-card-text>
                  </v-card>
                    <v-row justify="center">
                      <v-spacer></v-spacer>
                      <v-btn text tile href="https://github.com/zanniadevweb/plantGO_official" target="_blank">
                        <v-btn rounded small elevation="2" fab color="indigo">
                          <v-icon color="white">mdi-github</v-icon>
                        </v-btn>
                        <a>&nbsp;GitHub</a>
                      </v-btn>
                      <v-spacer></v-spacer>
                      <v-btn text tile href="https://trello.com/b/Kp12eugz/projet-tutor%C3%A9-s2-plantgo" target="_blank">
                        <v-btn rounded small elevation="2" fab color="indigo">
                          <v-icon color="white">mdi-trello</v-icon>
                        </v-btn>
                        <a>&nbsp;Trello</a>
                      </v-btn>
                      <v-spacer></v-spacer>
                      <v-btn text tile href="https://www.youtube.com/watch?v=JSq6NyNP-es" target="_blank">
                        <v-btn rounded small elevation="2" fab color="indigo">
                          <v-icon color="white">mdi-youtube</v-icon>
                        </v-btn>
                        <a>&nbsp;YouTube</a>
                      </v-btn>
                      <v-spacer></v-spacer>
                    </v-row>
                  </v-col>
                </v-row>
            <br><br>
            </v-card>
          <v-spacer></v-spacer>
          <v-spacer></v-spacer>
          </v-row>
        </v-card>
  </v-container>
</template>

<script>
export default {

  data: () => ({
    mobile: false,
  }),

  created () {
    // Si le format est trop étroit (ex: mobile), basculer le mode d'affichage du menu latéral
    if (this.$vuetify.breakpoint.mobile) {
      this.mobile = true
    } else {
      this.mobile = false
    }
  },

  computed: {
    largueurImageDesktop() {
      if (this.mobile) {
        return '100%'
      }
      else {
        return '25%'
      }
    },

    largueurTexteDesktop() {
      if (this.mobile) {
        return '100%'
      }
      else {
        return '60%'
      }
    },
  }
};
</script>
