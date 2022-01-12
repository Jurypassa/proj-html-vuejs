<template>
    <div>
        <div class="card borderpink" v-if="info.name == 'dj avada'">
            <img :src="require(`../../assets/img/${info.image}`)" :alt="info.name">
            <div class="testo">
                <p class="textpink">{{info.dj}}</p>
                <span>{{info.name}}</span>
                <button class="bgdcblue">view profile</button>
            </div>
        </div>
            <div class="card borderblue" v-else>
                <img :src="require(`../../assets/img/${info.image}`)" :alt="info.name"> 
                <div class="testo">
                    <p class="textblue">{{info.dj}}</p>
                    <span>{{info.name}}</span>
                    <button class="bgdcpink">view profile</button>
                </div>
            </div>
  </div>
</template>

<script>
export default {
    name: "CardDJ",
    props: {
        info: Object
    }

}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

    .card{
        position: relative;
        

        img{
            display: block;
            width: 100%;
            object-fit: cover;
        };

        .guest{
            object-position: top;
        }
    };

    .testo{
        position: absolute;
        top: 40px;
        left: 55px;

        p{
            text-transform: uppercase;
            font-size: 25px;
            letter-spacing: 2px;
            font-weight: bold;
        };

        span{
            display: block;
            display: block;
            font-size: 60px;
            padding-bottom: 20px;
        }
    };

    .textpink{
        color: $color-hot;
    };

    .bgdcpink{
        background-color: $color-hot;
    };

    .borderpink{
        border-top: 5px solid $color-hot;
    };
     .borderblue{
        border-top: 5px solid $color-cold;
    };

    .textblue{
        color: $color-cold;
    };

    .bgdcblue{
        background-color: $color-cold;
    }
</style>