<template>
  <v-container id='UXUI'>
    <v-card>
      <div class="mx-auto" style="width:1100px">
        <v-spacer></v-spacer>
        <v-card flat tile>
          <br><br>
            <v-card-title>
              <h2 class="subheading font-weight-bold mb-2">UX / UI&nbsp;</h2>
              <v-icon color="black">mdi-draw</v-icon>
            </v-card-title>
            <v-card color="blue lighten-5">
              <v-card-title>
                <v-btn text>
                <h3 style="font-size: 1.4em;">Application de gestion de véhicules (novembre 2020 - aujourd'hui)&nbsp;</h3>
                </v-btn>
              </v-card-title>
            </v-card>
            <v-row class="text-center">
              <v-col class="mb-5" cols="12">
                  <v-card flat tile>
                    <v-card-text style="font-size: 1.3em;line-height: 1.7em">
                      <p class="font-weight-regular" align="justify">
                        <b><i>Contexte</i></b> : Projet professionnel d'application Web. Le maquettage est réalisé avec Figma.
                        <br><br>
                        <b><i>Mon rôle</i></b> : Designer UX / UI.
                      </p>
                    </v-card-text>
                 </v-card>
             </v-col>
           </v-row>
        </v-card>
      </div>
      <v-spacer></v-spacer>
      <v-card flat tile>
        <v-carousel height="auto">
          <v-carousel-item src='../../public/images/pic06.jpg' reverse-transition="fade-transition" transition="fade-transition"><v-row class="mt-3" align="center" justify="center"><v-btn height="10%" color="blue"><div class="text-h2 white--text">Dasbhoard - Accueil</div></v-btn></v-row></v-carousel-item>
          <v-carousel-item src='../../public/images/pic07.jpg' reverse-transition="fade-transition" transition="fade-transition"><v-row class="mt-3" align="center" justify="center"><v-btn height="10%" color="blue"><div class="text-h2 white--text">Dasbhoard - Listing Réparations</div></v-btn></v-row></v-carousel-item>
          <v-carousel-item src='../../public/images/pic08.jpg' reverse-transition="fade-transition" transition="fade-transition"><v-row class="mt-3" align="center" justify="center"><v-btn height="10%" color="blue"><div class="text-h2 white--text">Dasbhoard - Détails Réparation</div></v-btn></v-row></v-carousel-item>
          <v-carousel-item src='../../public/images/pic09.jpg' reverse-transition="fade-transition" transition="fade-transition"><v-row class="mt-3" align="center" justify="center"><v-btn height="10%" color="blue"><div class="text-h2 white--text">Dasbhoard - Documents</div></v-btn></v-row></v-carousel-item>
          <v-carousel-item src='../../public/images/pic10.jpg' reverse-transition="fade-transition" transition="fade-transition"><v-row class="mt-3" align="center" justify="center"><v-btn height="10%" color="blue"><div class="text-h2 white--text">Messagerie</div></v-btn></v-row></v-carousel-item>
        </v-carousel>
      </v-card>
      <v-spacer></v-spacer>
    </v-card>
  </v-container>
</template>
