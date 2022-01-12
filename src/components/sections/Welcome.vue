<template>
  <section>

    <div class="container">

        <!-- inizio sezione welcome -->
        <div class="welcome">
            <h3>welcome to avada</h3>
            <h2>have the night of your life</h2>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Deleniti sed porro consectetur, fugit illum quas? Illum repellendus quisquam commodi iste nihil temporibus, fugit ducimus. Libero officiis repudiandae at mollitia vel.
            Tenetur autem unde animi. Illo doloribus consequuntur cupiditate dignissimos.</p>
        </div>
        <!-- fine sezione welcome -->
        
        <!-- inizio sezione card -->
        <div class="clearfix">
            <div class="cardwelcome" v-for="(card, index) in cards" :key="index">
                <Cardwelcome :info="card"/>
            </div>
        </div>
        
        <!-- fine sezione card -->
    </div>

    

  </section>
  
</template>

<script>
import Cardwelcome from "../elements/Cardwelcome.vue"

export default {
    name: "Welcome",
    components: {
        Cardwelcome
    },
    data() {
        return{
            cards: [
                {
                    image: "avada-nightclub-dancelounge-small.jpg",
                    name: "dance lounge"
                },
                {
                    image: "avada-nightclub-rooftoplounge-small.jpg",
                    name: "rooftop bar"
                },
                {
                    image: "avada-nightclub-viplounge-small.jpg",
                    name: "vip lounge"
                },
                {
                    image: "avada-nightclub-events-small.jpg",
                    name: "resident dj"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

    section{
        height: 1800px;
        background-image: url(../../assets/img/avada-nightclub-cloud-background.jpg);
        background-size: 125%;
        background-position-x: center;
    };

    .welcome{
        width: 70%;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 250px;

        h3{
            font-size: 24px;
            text-transform: uppercase;
            color: $color-cold;
            line-height: 0;
        }

        h2{
            font-size: 60px;
            line-height: 0;
            font-weight: normal;
        }

        p{
            text-align: center;
            font-size: 14px;
            padding-bottom: 40px
        }
    };


    .clearfix{
        margin-top: 50px;

        &:after{
        content: "";
        display: table;
        clear: both;
        }
    };
    

    .cardwelcome{
        width: 50%;
        float: left;
        
    }

</style>