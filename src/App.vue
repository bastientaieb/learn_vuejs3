<!--Gestion du HTML -->
<template>
  <main>
    <div id="app">
      <Home />
      <!-- Balise monofermente qui doit être au component appelé dans les exports -->
    </div>
  </main>
</template>

<!--Gestion du JS -->
<script>
// Import des components à dupliquer.
import Home from "./page/home.vue";

export default {
  name: "App",
  components: {
    Home,
  },
  // Instanciation des fichiers
};
</script>

<!--Gestion du CSS -->
<style>
@import "./style/reset.css";
/* Import du normalize */
@import url("https://fonts.googleapis.com/css2?family=Roboto%3Awght%40300%3B400%3B700&display=swap");
/* Import de la police */
#app {
  font-family: "Roboto", "sans-serif";
  padding: 0px 20px 0px 0px;
}
</style>
