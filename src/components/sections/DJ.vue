<template>
  <section>
      <CardDJ/>
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
        height: 300px;
    }
</style>