<template>
  <div class="back_footer">
    <Links />
    <Social />
  </div>
</template>

<script>
import Links from "./Content InfoLinks/Links.vue";
import Social from "./Content InfoLinks/Social.vue";

export default {
  name: "InfoLinks",

  components: {
    Links,
    Social,
  },
};
</script>


<style lang="scss">
.back_footer {
  background-color: #1e3120;
}
</style>