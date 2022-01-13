<template>
  <main>
      <Welcome/>
      <DJ/>
      <Diary/>
      <Exclusive/>
  </main>
</template>

<script>
import Welcome from "../sections/Welcome.vue";
import DJ from "../sections/DJ.vue";
import Diary from "../sections/Diary.vue";
import Exclusive from "../sections/Exclusive.vue";

export default {
    name: "Main",
    components: {
      Welcome,
      DJ,
      Diary,
      Exclusive
    }
}
</script>

<style lang="scss" scoped>

</style>