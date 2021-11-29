<template>
  <main>
    <Junbo />
    <ShowCase />
    <UsersTestimonials />
    <BestTips />
  </main>
</template>

<script>
import Junbo from "./Content Main/Junbo.vue";
import ShowCase from "./Content Main/Showcase.vue";
import UsersTestimonials from "./Content Main/UsersTestimonials.vue";
import BestTips from "./Content Main/BestTips.vue";

export default {
  name: "Main",

  components: {
    Junbo,
    ShowCase,
    UsersTestimonials,
    BestTips,
  },
};
</script>


<style scoped lang="scss">
</style>
