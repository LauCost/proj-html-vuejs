<template>
  <div class="back_green back_repeat_x negative_margin_top">
    <div class="cont_50 flex_between">
      <div
        class="card_icons"
        v-for="utilityPay in utilitysPay"
        :key="utilityPay.id"
      >
        <i :class="utilityPay.icon"></i>
        <p>
          {{ utilityPay.text }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "UtilityPay",

  data() {
    return {
      utilitysPay: [
        {
          id: 1,
          icon: "fas fa-truck",
          text: "Free Worldwide deliveries",
        },
        {
          id: 2,
          icon: "far fa-map",
          text: "Find stores near you",
        },
        {
          id: 3,
          icon: "fas fa-dollar-sign",
          text: "Best price guarranteed",
        },
        {
          id: 4,
          icon: "fas fa-credit-card",
          text: "All credit card accepted",
        },
      ],
    };
  },
};
</script>


<style lang="scss">
.negative_margin_top {
  margin-top: -4px;
}

.card_icons {
  padding: 50px 0;
  text-align: center;

  i {
    font-size: 55px;
    color: #fff;
  }

  p {
    margin-top: 20px;
    color: #9b9b9b;
    font-weight: bold;
  }
}
</style>