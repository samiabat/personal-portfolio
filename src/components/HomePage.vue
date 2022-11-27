<template>
  <v-app-bar color="indigo darken-2" app>
    <v-app-bar-nav-icon
          dark
          @click.stop="drawer = !drawer"
        >
      </v-app-bar-nav-icon>
    <v-toolbar-title>SAMUEL ABATNEH PORTFOLIO</v-toolbar-title>
    <v-spacer></v-spacer>

    <v-btn class="pr-5">
      <router-link to="/">Home</router-link>
    </v-btn>

    <v-btn to="/about" class="pr-5">
      About
    </v-btn>

    <v-btn class="pr-5">
      <v-text>Certeficates</v-text>
    </v-btn>

    <v-btn class="pr-5">
      <v-text>About</v-text>
    </v-btn>
    <v-btn class="pr-5">
      <v-text>Contact</v-text>
    </v-btn>
  </v-app-bar>
  <v-navigation-drawer
      v-model="drawer"
      absolute
      bottom
      temporary
    >
      HelloWorld
          
    </v-navigation-drawer>
</template>
<script>
  export default {
    data () {
      return {
        drawer: null,
        items: [
          { title: 'Home', icon: 'mdi-view-dashboard' },
          { title: 'About', icon: 'mdi-forum' },
        ],
      }
    },
  }
</script>