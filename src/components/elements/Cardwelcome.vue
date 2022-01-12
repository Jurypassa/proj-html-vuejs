<template>
  <div class="card">
      <img :src="require(`../../assets/img/${info.image}`)" :alt="info.name">

      <div class="name">
        <div class="text">
          <span>{{info.name}}</span>
        </div>
        <div class="border blu" v-show="info.name == 'dance lounge'"></div>
        <div class="border rosa" v-show="info.name == 'rooftop bar'"></div>
        <div class="border rosa" v-show="info.name == 'resident dj'"></div>
        <div class="border giallo" v-show="info.name == 'vip lounge'"></div>
      </div>
  </div>
</template>

<script>
export default {
    name: "Cardwelcome",
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
    }
  };

  .name{
    position: absolute;
    bottom: 45px;
    z-index: 2;
    font-size: 24px;
    font-weight: bold;
    width: 100%;
    line-height: 10px;
    display: flex;

    .text{
      width: 36%;
      text-align: right;

      span{
        display: inline-block;
      }
    }

    .border{
      width: 64%;
    };

    .blu{
      border-top: 1px solid $color-cold;
    };

    .rosa{
      border-top: 1px solid $color-hot;
    };

    .giallo{
      border-top: 1px solid rgb(206, 206, 9);
    };
  }
</style>