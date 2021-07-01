<template>
  <v-app>
    <v-app-bar
      app
      color="grey darken-4"
      dark
      dense
    >
      <v-toolbar-title>Alexandre ZANNI - Portfolio</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-app-bar-nav-icon @click.stop="mini = !mini"></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer
      v-model="drawer"
      dark
      permanent
      app
      right
      :mini-variant="mini"
      src="https://cdn.vuetifyjs.com/images/backgrounds/bg-2.jpg"
    >
    <v-card class="mx-auto" max-width="434" tile>
    <v-img v-if="!mini"
    height="100%"
    src="https://cdn.vuetifyjs.com/images/cards/server-room.jpg"
    >
    <v-col class="py-0">
        <v-list-item-content>
          <v-avatar size="128" v-if="!mini">
            <img
              src="@/images/photo_avatar.jpg"
              alt="John"
              tile
            >
        </v-avatar>
        </v-list-item-content>
    </v-col>
    <v-col class="py-0">
      <v-list-item
        color="rgba(0, 0, 0, .4)"
        dark
      >
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            Alexandre ZANNI
          </v-list-item-title>
          <v-list-item-title>Développeur Web Vue.js</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-col>
    </v-img>
    </v-card>
    <v-list nav dense>
<!--
<v-list-item v-for="item in items" :key="item.title" link @click="$vuetify.goTo('#Competences', options)">
  <v-list-item-icon>
    <v-icon>{{ item.icon }}</v-icon>
  </v-list-item-icon>

  <v-list-item-content>
    <v-list-item-title>{{ item.title }}</v-list-item-title>
  </v-list-item-content>
</v-list-item>
-->
      <v-list-item-group
        v-model="group"
        mandatory
        active-class="lime--text text--accent-4"
      >

        <v-list-item @click="$vuetify.goTo('#Presentation', options)">
          <v-list-item-icon>
            <v-icon>mdi-card-text-outline</v-icon>
          </v-list-item-icon>
          <v-list-item-title>Présentation</v-list-item-title>
        </v-list-item>

        <v-list-item @click="$vuetify.goTo('#Competences', options)">
          <v-list-item-icon>
            <v-icon>mdi-account-cog</v-icon>
          </v-list-item-icon>
          <v-list-item-title>Compétences</v-list-item-title>
        </v-list-item>

          <v-list-item @click="$vuetify.goTo('#Web', options)">
            <v-list-item-icon>
              <v-icon>mdi-web</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Web</v-list-item-title>
          </v-list-item>

          <v-list-item @click="$vuetify.goTo('#Mobile', options)">
            <v-list-item-icon>
              <v-icon>mdi-android</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Mobile</v-list-item-title>
          </v-list-item>

          <v-list-item @click="$vuetify.goTo('#UXUI', options)">
            <v-list-item-icon>
              <v-icon>mdi-draw</v-icon>
            </v-list-item-icon>
            <v-list-item-title>UX / UI</v-list-item-title>
          </v-list-item>

          <v-list-item @click="$vuetify.goTo('#Contact', options)">
            <v-list-item-icon>
              <v-icon>mdi-email</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Contact</v-list-item-title>
          </v-list-item>

      </v-list-item-group>
    </v-list>
    </v-navigation-drawer>

    <v-main>
      <Presentation/>
      <Competences/>
      <Web/>
      <Mobile/>
      <UXUI/>
    </v-main>

    <v-bottom-navigation color="grey darken-4" dark id='Contact'>
        <span class="font-weight-bold white--text mt-4">
          zannialexandre245@gmail.com&nbsp;
          <v-icon>mdi-email</v-icon>
        </span>
        <span>
          <v-row justify="center" class="ml-5 mt-3">
              <v-spacer></v-spacer>
            <v-btn text tile href="mailto:zannialexandre245@gmail.com">
              <v-btn rounded small elevation="2" fab color="indigo">Mail
                <v-icon color="white">
                  mdi-email
                </v-icon>
              </v-btn>
            </v-btn>
              <v-spacer></v-spacer>
            <v-btn text tile href="https://www.linkedin.com/in/alexandre-zanni-232884187">
              <v-btn rounded small elevation="2" fab color="indigo">Linkedin
                <v-icon color="white">
                  mdi-linkedin
                </v-icon>
              </v-btn>
            </v-btn>
              <v-spacer></v-spacer>
            <v-btn text tile href="https://www.instagram.com/archaeology_in_sicily/">
              <v-btn rounded small elevation="2" fab color="indigo">Instagram
                <v-icon color="white">
                  mdi-instagram
                </v-icon>
              </v-btn>
            </v-btn>
              <v-spacer></v-spacer>
          </v-row>
        </span>

      <!--
      <v-btn click="copierTexte" v-model="texte" color="indigo" class="white-text">
        Copier
      </v-btn>
      -->
    </v-bottom-navigation>
  </v-app>
</template>

<!-- Scrolling Refs : https://vuetifyjs.com/en/features/scrolling/ -->
<script>
import Presentation from './components/Presentation';
import Competences from './components/Competences';
import Web from './components/Web';
import Mobile from './components/Mobile';
import UXUI from './components/UXUI';
import * as easings from 'vuetify/es5/services/goto/easing-patterns';

export default {
  name: 'App',

  components: {
    Presentation,
    Competences,
    Web,
    Mobile,
    UXUI,
  },

  data: () => ({
    drawer: false,
    group: null,
    type: 'number',
    number: 9999,
    duration: 300,
    offset: 0,
    easing: 'easeInOutQuint',
    easings: Object.keys(easings),
    mini: false,
    texte: 'zannialexandre245@gmail.com'
/*
items: [
  { title: "Présentation", icon: "mdi-card-text-outline", tag_link:"Competences"},
  { title: "Compétences", icon: "mdi-account-cog" },
  { title: "Web", icon: "mdi-web" },
  { title: "Mobile", icon: "mdi-android" },
  { title: "UX / UI", icon: "mdi-draw" },
  { title: "Contact", icon: "mdi-email" },
],
*/
  }),

  computed: {
    tailleAvatar() {
      return 30;
    },
    target () {
      const value = this[this.type]
      if (!isNaN(value)) return Number(value)
      else return value
    },
    options () {
      return {
        duration: this.duration,
        offset: this.offset,
        easing: this.easing,
      }
    },
    element () {
      if (this.selected === 'Button') return this.$refs.button
      else if (this.selected === 'Radio group') return this.$refs.radio
      else return null
    }
  },

  methods: {
    copierTexte() {
      navigator.clipboard.writeText(this.texte)
    }
  }
};
</script>
