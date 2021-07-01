<template>
  <v-container id='Mobile'>
      <v-card class="mx-auto">
        <v-card flat tile class="mx-auto" style="width:1100px">
        <br><br>
          <v-card-text style="font-size: 1.1em">
            <h2 class="subheading font-weight-bold mb-2">
              Mobile
            </h2>
          </v-card-text>

          <v-row class="text-center">
            <v-col
              class="mb-5"
              cols="12"
            >

            <v-card flat tile class="mx-auto" style="width:1100px">
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
                <v-btn text tile href="https://github.com/zanniadevweb/plantGO_official">
                  <v-btn rounded small elevation="2" fab color="indigo">
                    <v-icon color="white">
                      mdi-github
                    </v-icon>
                  </v-btn>
                  <a
                  >
                    &nbsp;GitHub
                  </a>
                </v-btn>
                  <v-spacer></v-spacer>
                <v-btn text tile href="https://trello.com/b/Kp12eugz/projet-tutor%C3%A9-s2-plantgo">
                  <v-btn rounded small elevation="2" fab color="indigo">
                    <v-icon color="white">
                      mdi-trello
                    </v-icon>
                  </v-btn>
                  <a
                  >
                    &nbsp;Trello
                  </a>
                </v-btn>
                  <v-spacer></v-spacer>
                <v-btn text tile href="https://www.youtube.com/watch?v=JSq6NyNP-es">
                  <v-btn rounded small elevation="2" fab color="indigo">
                    <v-icon color="white">
                      mdi-youtube
                    </v-icon>
                  </v-btn>
                  <a
                  >
                    &nbsp;YouTube
                  </a>
                </v-btn>
                  <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
      <br><br>
      </v-card>
      </v-card>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
    })
  }
</script>
