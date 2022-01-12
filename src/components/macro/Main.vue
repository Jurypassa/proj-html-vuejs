<template>
  <main>
      <Welcome/>
      <DJ/>
      <Diary/>
  </main>
</template>

<script>
import Welcome from "../sections/Welcome.vue";
import DJ from "../sections/DJ.vue";
import Diary from "../sections/Diary.vue";

export default {
    name: "Main",
    components: {
      Welcome,
      DJ,
      Diary
    }
}
</script>

<style lang="scss" scoped>

</style>