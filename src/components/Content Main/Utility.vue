<template>
  <div>
    <UtilityProduction />
    <UtilityPay />
  </div>
</template>

<script>
import UtilityProduction from "./Content Utility/UtilityProduction.vue";
import UtilityPay from "./Content Utility/UtilityPay.vue";

export default {
  name: "utility",

  components: {
    UtilityProduction,
    UtilityPay,
  },
};
</script>