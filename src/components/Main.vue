<template>
  <main>
    <Junbo />
    <ShowCase />
    <UsersTestimonials />
    <BestTips />
    <Utility />
  </main>
</template>

<script>
import Junbo from "./Content Main/Junbo.vue";
import ShowCase from "./Content Main/Showcase.vue";
import UsersTestimonials from "./Content Main/UsersTestimonials.vue";
import BestTips from "./Content Main/BestTips.vue";
import Utility from "./Content Main/Utility.vue";

export default {
  name: "Main",

  components: {
    Junbo,
    ShowCase,
    UsersTestimonials,
    BestTips,
    Utility,
  },
};
</script>


<style scoped lang="scss">
</style>
