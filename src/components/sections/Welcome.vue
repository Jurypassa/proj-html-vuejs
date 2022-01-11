<template>
  <section>

      <div class="container">

          <!-- inizio sezione welcome -->
            <div class="welcome">
                <h3>welcome to avada</h3>
                <h2>have the night of your life</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Neque numquam voluptatem excepturi obcaecati ea optio similique odio corporis, ipsa eligendi impedit deleniti nemo sapiente quaerat nisi voluptates! Fuga, aliquid vero.</p>
            </div>
      <!-- fine sezione welcome -->

      </div>
      
      

  </section>
</template>

<script>
export default {
    name: "Welcome"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

    section{
        height: 1500px;
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
        }
    }
</style>