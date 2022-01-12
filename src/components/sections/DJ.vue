<template>
  <section>
      
      <div class="CardDJ" v-for="(card, index) in cards" :key="index">
          <CardDJ :info="card"/>
      </div>
  </section>
</template>

<script>
import CardDJ from "../elements/CardDJ.vue";

export default {
    name: "DJ",
    components: {
        CardDJ
    },
    data() {
        return{
            cards: [
                {
                    image: "avada-nightclub-resident-profile.jpg",
                    dj: "resident dj",
                    name: "dj avada"
                },
                {
                    image: "avada-nightclub-lisahouse-inset-new.jpg",
                    dj: "special guest dj",
                    name: "dj blondie"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section{
        display: flex;
        width: 100%;
        height: 700px;
        overflow: hidden;
    }
</style>