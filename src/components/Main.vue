<template>
  <main>
    <Junbo />
    <ShowCase />
    <UsersTestimonials />
    <BestTips />
    <Utility />
    <NewProduction />
  </main>
</template>

<script>
import Junbo from "./Content Main/Junbo.vue";
import ShowCase from "./Content Main/Showcase.vue";
import UsersTestimonials from "./Content Main/UsersTestimonials.vue";
import BestTips from "./Content Main/BestTips.vue";
import Utility from "./Content Main/Utility.vue";
import NewProduction from "./Content Main/NewProduction.vue";

export default {
  name: "Main",

  components: {
    Junbo,
    ShowCase,
    UsersTestimonials,
    BestTips,
    Utility,
    NewProduction,
  },
};
</script>


<style scoped lang="scss">
</style>
