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

      <!-- inizio sezione memories -->
      <div class="memories">
          <h2>making memories all night long</h2>
      </div>
      <!-- fine sezione memories -->

      <!-- inizio sezione bottone -->
      <div class="button">
        <button>
          become a vip
        </button>
      </div>
      <!-- fine sezione bottone -->

      <!-- inizio sezione view -->
      <div class="view">
          <img src="../../assets/img/avada-nightclub-play-showreel-400x95.png" alt="">
      </div>
      <!-- fine sezione view -->






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
@import "../../assets/style/partials/variable.scss";

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
        display: block;
    };

    .memories{
        height: 220px;
        background-color: rgba($color: #000000, $alpha: 0.9);
        border-top: 5px solid $color-cold;
        display: flex;
        justify-content: center;
        align-items: center;
    };

    h2{
        font-size: 50px;
    };

    .button{
        text-align: center;
        margin-top: -30px;
        
        button{
            background-color: $color-hot;
        }
    };

    .view{
        text-align: center;
        padding-top: 60px;

        img{
            width: 23%;
        }
    }
</style>