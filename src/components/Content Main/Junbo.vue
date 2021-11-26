<template>
  <div class="back_green">
    <div class="cont_50 flex_space_between">
      <p class="info_junbo">
        <span> <i class="far fa-map"></i> International </span>
        Shipping Services
      </p>
      <p class="info_junbo">
        <i class="far fa-clock"></i> See our
        <span> store hours </span>
        and services
      </p>
      <p class="info_junbo">
        <i class="fas fa-check"></i> We price match to give you the
        <span> best deals </span>
      </p>
    </div>
    <div class="junboImg">
      <div class="cont_70"></div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Junbo",
};
</script>


<style lang="scss">
.back_green {
  background-color: #1e3120;
  background-image: url(../../assets/img/bg-transparent-3.png);
}

.cont_50 {
  width: 50%;
  margin: auto;
  padding: 20px 0;
}

.info_junbo {
  color: #fff;
  span {
    color: #fff;
    font-weight: bold;
  }
}
</style>