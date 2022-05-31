<template>
  <div class="restaurants">
    <h2 class="restaurants__title">Populaires à proximité</h2>
    <div class="restaurants__nearby">
      <RestaurantCard v-for="(card, index) in 3" :key="index" />
      <!-- Création de 3 restaurant card -->
    </div>
  </div>
</template>

<script>
import RestaurantCard from "./RestaurantCard.vue";
export default {
  name: "RestaurantRow",
  components: {
    RestaurantCard,
  },
};
</script>

<style lang="scss">
.restaurants {
  .restaurants__title {
    margin-left: 40px;
    font-size: 2rem;
  }
  .restaurants__nearby {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }
}
</style>
