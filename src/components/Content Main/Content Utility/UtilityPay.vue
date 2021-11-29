<template>
  <div class="back_green back_repeat_x">
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
      ],
    };
  },
};
</script>