<template>
  <header id="header">

      <div class="container">
          
      <!-- inizio sezione navbar -->
        <div class="nav">
            <Barra/>
        </div>
      <!-- fine sezione navbar -->

      <!-- inizio sezione Hero -->
      <div class="hero">
          <img src="../../assets/img/avada-nightclub-homepage-image.png" alt="home page image">
      </div>
      <!-- fine sezione Hero -->



      </div>
  </header>
</template>

<script>
import Barra from "../elements/Barra.vue"

export default {
    name: "Header",
    components: {
        Barra,
    }
}
</script>

<style lang="scss" scoped>
    #header{
        height: 1300px;
        background-image: url(../../assets/img/avada-nightclub-home-hero.jpg);
        background-size: cover;
    };

    .nav{
        padding-top: 20px;
    };

    .hero img{
        width: 100%;
        padding-top: 50px;
    }
</style>