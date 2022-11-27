<template>
  <v-app>
    <v-main>
      <HomePage />
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HomePage from './components/HomePage.vue'

export default {
  name: 'App',

  components: {
    // HelloWorld,
    HomePage,
  },

  data: () => ({
    //
  }),
}
</script>
<style>
</style>
