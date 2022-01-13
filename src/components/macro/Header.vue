<template>
    <header id="header">

        <!-- inizio sezione carrello -->
        <div class="squares">

            <div class="square uno">
                <i class="grey fas fa-laptop"></i>
                <p class="grey">Demos</p>
            </div>

            <div class="square due">

                <div class="saldi">
                    <i class="green dollaro fas fa-dollar-sign"></i>
                    <span class="green">39</span>
                </div>

                <p class="grey">On sale</p>

            </div>
        </div>
        <!-- fine sezione carrello -->


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

    .squares{
        position: fixed;
        z-index: 2;
        top: 170px;
        right: 20px;

        .square{
            background-color: white;
            margin-bottom: 5px;
            width: 80px;
            height: 80px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            border-radius: 10px;
            
            p{
                color: black;
                font-size: 12px;
                font-weight: bold;
                letter-spacing: 1px;
                margin: 0;
            }
        }
    };

    .uno{
        
        .grey{
            font-size: 30px;
        }
    };

    .saldi{
        padding-right: 5px;
        .dollaro{
            vertical-align: top;
            padding-top: 8px;
        }

        span{
            font-size: 30px;
        }
    }

    .grey{
        color: #33475b;
    };

    .green{
        color: green;
        font-weight: bold;
    }

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

            &:hover{
            background-color: $hot-hover;
        }
        };

        
    };

    .view{
        text-align: center;
        padding-top: 60px;

        img{
            width: 23%;
            cursor: pointer;
        }
    }
</style>