<template>
  <v-container id='Competences'>
    <v-card class="mx-auto">
      <v-row align="center" justify="center" dense>
        <v-card flat tile class="mx-auto" style="width:1100px">
        <br><br>
          <v-card-title>
            <h2 class="subheading font-weight-bold mb-2">Compétences&nbsp;</h2>
            <v-icon color="black">  mdi-account-cog</v-icon>
          </v-card-title>
          <v-card-title>
            <h3 class="subheading font-weight-bold mb-2">Fonctionnelles</h3>
          </v-card-title>
          <br><br>
          <v-row class="text-center">
            <v-col class="mb-5" cols="12">
              <v-row justify="center">
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-account-group</v-icon>
                  </v-avatar>
                    &nbsp;COO (UML)
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-git</v-icon>
                  </v-avatar>
                    &nbsp;Git
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-draw</v-icon>
                  </v-avatar>
                    &nbsp;Maquettage UX/UI
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white"> mdi-trello</v-icon>
                  </v-avatar>
                    &nbsp;Gestion de Projet
                </span>
                <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
          <br><br>
          <v-card-title>
            <h3 class="subheading font-weight-bold mb-2">Techniques : Bureautique</h3>
          </v-card-title>
          <br><br>
          <v-row class="text-center">
            <v-col
              class="mb-5"
              cols="12"
            >
              <v-row justify="center">
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-github</v-icon>
                  </v-avatar>
                    &nbsp;HTML5/CSS3
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-format-font</v-icon>
                  </v-avatar>
                    &nbsp;Suite Microsoft
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-vector-difference-ab</v-icon>
                  </v-avatar>
                    &nbsp;Figma
                </span>
                <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
          <br><br>
          <v-row class="text-center">
            <v-col
              class="mb-5"
              cols="12"
            >
              <v-row justify="center">
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-adobe</v-icon>
                  </v-avatar>
                    &nbsp;Adobe Illustrator / Photoshop
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-wordpress</v-icon>
                  </v-avatar>
                    &nbsp;WordPress
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-google-maps</v-icon>
                  </v-avatar>
                    &nbsp;ArcGIS / QGIS
                </span>
                <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
          <br><br>
          <v-card-title>
            <h3 class="subheading font-weight-bold mb-2">Techniques : Informatique</h3>
          </v-card-title>
          <br><br>
          <v-row class="text-center">
            <v-col
              class="mb-5"
              cols="12"
            >
              <v-row justify="center">
                  <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-database</v-icon>
                  </v-avatar>
                    &nbsp;MySQL, IndexedDB
                </span>
                  <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-android</v-icon>
                  </v-avatar>
                    &nbsp;POO : Java, C++
                </span>
                  <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-web</v-icon>
                  </v-avatar>
                    &nbsp;Javascript (Vue.js), PHP (Symfony)
                </span>
                  <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-linux</v-icon>
                  </v-avatar>
                    &nbsp;Linux, Bash
                </span>
                  <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
          <br><br>
          <v-card-title>
            <h3 class="subheading font-weight-bold mb-2">Qualités humaines</h3>
          </v-card-title>
          <br><br>
          <v-row class="text-center">
            <v-col class="mb-5" cols="12">
              <v-row justify="center">
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white"> mdi-account-multiple-plus</v-icon>
                  </v-avatar>
                    &nbsp;Travail en équipe
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-btn rounded small elevation="2" fab color="indigo">
                    <v-icon color="white">mdi-emoticon</v-icon>
                  </v-btn>
                    &nbsp;Optimisme
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-glasses</v-icon>
                  </v-avatar>
                    &nbsp;Consciencieux
                </span>
                <v-spacer></v-spacer>
                <span>
                  <v-avatar color="indigo">
                    <v-icon color="white">mdi-graph</v-icon>
                  </v-avatar>
                    &nbsp;Sérieux et organisé
                </span>
                <v-spacer></v-spacer>
              </v-row>
            </v-col>
          </v-row>
          <br><br>
        </v-card>
      </v-row>
    </v-card>
  </v-container>
</template>
