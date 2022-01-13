<template>
  <section>
      <div class="contenitore">

        <!-- inizio sezione immagine -->
        <div class="image">
            <img :src="require(`../../assets/img/${info.image}`)" :alt="info.name">
        </div>
        <!-- inizio sezione immagine -->

        <!-- inizio sezione testo -->
        <div class="testo">
          <p class="night">{{info.event}}</p>
          <p class="month">{{info.month}}</p>
        </div>
        <!-- inizio sezione testo -->

      </div>
  </section>
</template>

<script>
export default {
    name: "Cardevents",
    props: {
      info: Object
    }
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";


  .contenitore{
    display: flex;
    justify-content: center;
    padding: 10px 0;
  }

  .image{

    img{
      object-position: center;
      padding-top: 15px;
      cursor: pointer;
    }
  };

  .testo{
    padding-left: 15px;
    padding-top: 15px;
    cursor: pointer;

    .night{
    color: $color-cold;
    font-size: 25px;
    margin: 0;
    font-weight: bold
  };

  .month{
    font-size: 14px;
    font-weight: bold;
    color: $color-footer;
    margin: 0;
  }
  }

  
</style>