<template>
  <section>

      <div class="container">

          <!-- inizio sezione Diary -->
      <span class="events">special events</span>
      <span class="diary">for your diary</span>
      <!-- fine sezione Diary -->
      
      <!-- inizio sezione Card -->
      <div class="clearfix">
            <div class="card" v-for="(card, index) in cards" :key="index">
                <CardDiary :info="card"/>
            </div>
      </div>
      <!-- fine sezione Card -->

      <!-- inizio sezione bottone -->
      <div class="button">
          <button>rsvp now</button>
      </div>
      <!-- fine sezione bottone -->


      </div>

      

      
  </section>
</template>

<script>
import CardDiary from "../elements/CardDiary.vue";

export default {
    name: "Diary",
    components: {
        CardDiary
    },
    data() {
        return {
            cards: [
                {
                    image: "avada-nightclub-events-6-800x450.jpg",
                    night: "DJ Fusion",
                    month: "August 19 @ 8:00 am"
                },
                {
                    image: "avada-nightclub-events-5-800x450.jpg",
                    night: "House Nation",
                    month: "August 19 @ 8:00 am"
                },
                {
                    image: "avada-nightclub-events-4-800x450.jpg",
                    night: "Jazz Night",
                    month: "August 19 @ 8:00 am"
                },
                {
                    image: "avada-nightclub-events-3-800x450.jpg",
                    night: "VIP Tastier Sessions",
                    month: "September 1 @ 8:00 am"
                },
                {
                    image: "avada-nightclub-events-2-800x450.jpg",
                    night: "Funky House Rave",
                    month: "September 16 @ 8:00 am"
                },
                {
                    image: "avada-nightclub-events-1-800x450.jpg",
                    night: "Urban Vibes",
                    month: "September 20 @ 8:00 am"
                },
                
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

    section{
        background-image: url(../../assets/img/avada-nightclub-homepage-events-background-new.jpg);
        height: 1700px;
        background-size: 170%;
        background-position-x: center;
    };


    span{
        display: block;
        text-align: center;
    };

    .events{
        color: $color-hot;
        text-transform: uppercase;
        padding-top: 330px;
        font-size: 23px;
        font-weight: bold;
        letter-spacing: 2px;
    };

    .diary{
        font-size: 60px;
    };

    .clearfix{
        padding-top: 70px;
    }

    .clearfix:after{
        content: "";
        display: table;
        clear: both;
    }

    .card{
        float: left;
        width: calc(100% / 3 - 40px);
        padding: 35px 20px;
    };

    .button{
        text-align: center;
        padding-top: 50px;

        button{
        background-color: $color-hot;
        font-size: 18px;

            &:hover{
                background-color: $hot-hover;
            }
        }
    }

    
</style>