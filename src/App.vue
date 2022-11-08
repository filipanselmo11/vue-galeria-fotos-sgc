<template>
  <v-app>
    <v-app-bar app color="light-blue darken-2" dark> </v-app-bar>

    <v-main>
      <br/>
      <home-page></home-page>
    </v-main>
  </v-app>
</template>

<script>
import HomePage from './components/HomePage.vue'
export default {
  name: "App",

  components: {HomePage},

  data: () => ({
    //
  }),
};
</script>

<style scoped>
.v-main {
  margin: 0 !important;
  /* background: yellow !important; */
  box-sizing: border-box !important;
}
</style>