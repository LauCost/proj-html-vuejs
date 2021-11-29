<template>
  <div class="back_footer">
    <Links />
  </div>
</template>

<script>
import Links from "./Content InfoLinks/Links.vue";

export default {
  name: "InfoLinks",

  components: {
    Links,
  },
};
</script>


<style lang="scss">
.back_footer {
  background-color: #1e3120;
}
</style>