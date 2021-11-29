<template>
  <main>
    <Junbo />
    <ShowCase />
    <UsersTestimonials />
  </main>
</template>

<script>
import Junbo from "./Content Main/Junbo.vue";
import ShowCase from "./Content Main/Showcase.vue";
import UsersTestimonials from "./Content Main/UsersTestimonials.vue";

export default {
  name: "Main",

  components: {
    Junbo,
    ShowCase,
    UsersTestimonials,
  },
};
</script>


<style scoped lang="scss">
</style>
