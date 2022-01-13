<template>
  <footer>
      <div class="container">
        
        <!-- inizio sezione Card -->
        <div class="events size">
          <span class="uppercase">events</span>
          <div class="card" v-for="(card, index) in  cards" :key="index">
            <Cardevents :info="card"/>
          </div>
          <p>View All Events</p>
        </div>
        <!-- fine sezione Card -->

        <!-- inizio sezione info -->
        <div class="info size">

          <!-- inizio logo -->
          <img src="../../assets/img/avada-nightclub-logo-2x-300x99.png" alt="logo night club">
          <!-- fine logo -->

          <!-- inizio contatti -->
          <div class="contact">
            <p class="gray">Avada NightClub</p>
            <p class="gray">100 Night Club Blvd</p>
            <p class="gray">Beverly Hills</p>
            <p class="blue">hi@your-domains.com</p>
            <p class="gray">+1 (555) 000 000</p>
          <!-- fine contatti -->

          <!-- inizio icone -->
          <div class="icone">
            <i class="fab fa-facebook-f"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-youtube"></i>
          </div>
          <!-- fine icone -->

          </div>
          
        </div>
        <!-- fine sezione info -->

        <!-- inizio sezione foto -->
        <div class="foto size">
          <span class="uppercase">venus</span>
          <img src="../../assets/img/avada-nightclub-footer-rooftop-400x171.jpg" alt="rooftop bar">
          <img src="../../assets/img/avada-nightclub-footer-dancelounge-400x171.jpg" alt="dance lounge">
        </div>
        <!-- fine sezione foto -->

      </div>

      <!-- inizio sezione copyright -->
      <div class="copyright">
        <i class="far fa-copyright"></i>
        <p>Copyright 2012 - 2022 | </p>
        <p>Avada Theme by <span class="blue">ThemeFusion</span> | </p>
        <p>All Rights Reserved | </p>
        <p>Powered by <span class="blue">WordPress</span></p>
      </div>
      <!-- fine sezione copyright -->

      <!-- inizio sezione anchor -->
      <div class="anchor">
        <a href="#header"><i class="arrow fas fa-chevron-up"></i></a>
      </div>
      
      <!-- fine sezione anchor -->
      
  </footer>
</template>

<script>
import Cardevents from "../elements/Cardevents.vue"

export default {
    name: "Footer",
    components: {
      Cardevents
    },
    data() {
      return{
        cards: [
          {
            image: "avada-nightclub-events-6-66x66.jpg",
            event: "DJ Fusion",
            month: "August 19 @ 8:00 am"
          },
          {
            image: "avada-nightclub-events-5-66x66.jpg",
            event: "House Nation",
            month: "August 19 @ 8:00 am"
          },
          {
            image: "avada-nightclub-events-4-66x66.jpg",
            event: "Jazz Night",
            month: "August 19 @ 8:00 am"
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

footer{
  background-image: url(../../assets/img/avada-nightclub-footer-background-final-2.jpg);
  background-position-y: bottom;
  height: 750px;
  background-size: cover;
  position: relative
};

.size{
  width: calc(100% / 3);
  text-align: center;
}

.container{
  display: flex;
  padding-top: 50px;
}

.uppercase{
  text-transform: uppercase;
  margin-top: 50px;
  display: block;
  font-size: 18px;
}

.events{
  p{
    color: $color-cold;
  }
};

.blue{
  color: $color-cold;
  cursor: pointer;
};

.gray{
  color: gray;
}

.contact{
  padding-top: 40px;

  p{
    margin: 0;
    padding-bottom: 5px
  }
};

.icone{
  padding-top: 40px;
  cursor: pointer;

  &>*{
    padding: 15px;
  }
};

.foto{
  
  img{
    padding-top: 30px;
    cursor: pointer;
  }
};

.copyright{
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 12px;
  color: $color-footer;
  margin-top: 130px;
};

.anchor{
  position: absolute;
  bottom: 30px;
  right: 100px;
}

.arrow{
  color: white;
  background-color: #363636;
  padding: 18px;
}

</style>