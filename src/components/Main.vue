<template>
  <main>
    <Junbo />
    <ShowCase />
  </main>
</template>

<script>
import Junbo from "./Content Main/Junbo.vue";
import ShowCase from "./Content Main/Showcase.vue";

export default {
  name: "Main",

  components: {
    Junbo,
    ShowCase,
  },
};
</script>


<style scoped lang="scss">
</style>
