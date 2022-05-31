<template>
  <div class="home">
    <RestaurantRow />
  </div>
</template>

<script>
// import de la base de données
import bdd from "../bdd.js";
// Components
import RestaurantRow from "../components/RestaurantRow.vue";
export default {
  name: "Home",
  components: {
    RestaurantRow,
  },
  // Gestion du JS (Fonctions, data,)
  setup() {
    class Restaurant {
      constructor(name, note, image, drive_time) {
        (this.name = name),
          (this.note = note),
          (this.image = image),
          (this.drive_time = drive_time);
      }
      // La Class va regrouper tous les éléments des restaurants qui correspondent à ce qu'on retrouve dans la BDD. 
      // This permet de rendre dynamique les éléments du constructor des restaurants
    }
  },
};
</script>

<style lang="scss"></style>
