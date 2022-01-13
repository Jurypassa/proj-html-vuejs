<template>
  <nav id="navbar">
    <h4>home</h4>
    <h4>the club</h4>
    <h4>events</h4>
    <img src="../../assets/img/avada-nightclub-logo-2x-400x132.png" alt="logo">
    <h4>jobs</h4>
    <h4>news</h4>
    <h4>contact us</h4>
  </nav>
</template>

<script>
export default {
    name: "Barra"
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/partials/variable.scss";

  h4{
    display: inline-block;
    text-transform: uppercase;
    margin-top: 50px;
    font-weight: bold;
    cursor: pointer;
    padding-bottom: 15px;

    &:hover{
      color: $color-hot;
      border-bottom: 3px solid $color-hot;
    }
  };

  img{
    cursor:pointer;
  }

  #navbar{
    height: 132px;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
</style>