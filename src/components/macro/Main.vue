<template>
  <main>
      <Welcome/>
      <DJ/>
  </main>
</template>

<script>
import Welcome from "../sections/Welcome.vue";
import DJ from "../sections/DJ.vue";

export default {
    name: "Main",
    components: {
      Welcome,
      DJ
    }
}
</script>

<style lang="scss" scoped>

</style>