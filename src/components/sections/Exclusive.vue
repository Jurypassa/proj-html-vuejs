<template>
  <section>

    <div class="container">

      <!-- inizio sezione testo -->
      <div class="text">
        <p class="tonight">become a vip tonight</p>
        <p class="lounge">exclusive vip lounge</p>
      </div>
      <!-- fine sezione testo -->

      <!-- inizio sezione bottone -->
      <div class="button">
        <button>join the club</button>
      </div>
      <!-- fine sezione bottone -->
    </div>
  </section>
</template>

<script>
export default {
    name: "Exclusive"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

  section{
    background-image: url(../../assets/img/avada-nightclub-vip-hero-new.jpg);
    height: 300px;
    background-size: 70%;
  };

  .container{
    display: flex;
    height: 100%;
    align-items: center
  };

  .text{
    width: 70%;
    padding-left: 130px;

    .tonight{
      color: $color-cold;
      text-transform: uppercase;
      font-size: 20px;
      font-weight: bold;
      letter-spacing: 1px;
      line-height: 0;
    }

    .lounge{
      font-size: 60px;
      line-height: 0;
    }
  };

  .button{
    width: 30%;

    button{
      background-color: $color-hot;
      font-size: 18px;

      &:hover{
        background-color: $hot-hover;
      }
    }
  }
</style>