<template>
  <div>
      <div class="card">
        <img :src="require(`../../assets/img/${info.image}`)" :alt="info.name">
        <span class="night">{{info.night}}</span>
        <span class="month">{{info.month}}</span>
      </div>
  </div>
</template>

<script>
export default {
    name: "CardDiary",
    props: {
      info: Object
    }
}
</script>
    

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

  .card{

    img{
      width: 100%;
      cursor: pointer;
    };

    span{
      display: block;
      cursor: pointer;
    }
  };

  .night{
    color: $color-hot;
    font-size: 23px;
    font-weight: bold;
    padding-left: 20px;
    padding-top: 20px;
  };

  .month{
    padding-left: 20px;
    font-size: 12px;
    font-weight: bold;

  }
</style>