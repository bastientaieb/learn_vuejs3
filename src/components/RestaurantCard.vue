<script>
export default { name: "RestaurantCard" };
</script>

<template>
  <div class="restaurant-card">
    <div class="restaurant-card__restaurant-image"></div>
    <div class="restaurant-card__restaurant-information">
      <div class="information-top">
        <p class="information-top__name">Subway</p>
        <p class="information-top__rate">4.5</p>
      </div>
      <p class="information-bottom">20-30 min</p>
    </div>
  </div>
</template>

<style lang="scss">
.restaurant-card {
  width: 32%;
  height: 30vh;
  margin-left: 40px;
  .restaurant-card__restaurant-image {
    background-image: url("https://cn-geo1.uber.com/image-proc/resize/eats/format=webp/width=550/height=440/quality=70/srcb64=aHR0cHM6Ly9kMXJhbHNvZ25qbmczNy5jbG91ZGZyb250Lm5ldC8zNzg4MDJiMC1jNTI4LTQ4MjktYjBiNS0wY2M2NDBkZjYzY2QuanBlZw==");
    height: 70%;
    background-position: center;
    background-size: cover;
  }
  .restaurant-card__restaurant-information {
    .information-top {
      display: flex;
      justify-content: space-between;
      align-items: center;
      .information-top__name {
        font-size: 1.2rem;
        font-weight: 600;
      }
      .information-top__rate {
        width: 35px;
        height: 35px;
        border-radius: 18px;
        background: #eeeeee;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 0.9rem;
      }
    }
    .information-bottom {
      font-size: 0.9rem;
      margin-top: 0px;
    }
  }
}
</style>
