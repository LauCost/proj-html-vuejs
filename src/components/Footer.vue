<template>
  <footer>
    <InfoLinks />
    <Copyright />
  </footer>
</template>


<script>
import InfoLinks from "./Content Footer/InfoLinks.vue";
import Copyright from "./Content Footer/Copyright.vue";

export default {
  name: "Footer",

  components: {
    InfoLinks,
    Copyright,
  },
};
</script>