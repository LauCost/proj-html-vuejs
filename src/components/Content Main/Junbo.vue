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
      <div class="cont_70_pad">
        <p>FIND THE BEST ANIMAL SUPPLIES</p>
        <h2>
          We Know animals are a part of your family, let us help take care of
          them.
        </h2>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Junbo",
};
</script>


<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display&family=Source+Sans+Pro:wght@200&display=swap");
.back_green {
  background-color: #1e3120;
  background-image: url(../../assets/img/bg-transparent-3.png);
}

.cont_50 {
  width: 50%;
  margin: auto;
  padding: 20px 0;
}

.cont_70_pad {
  width: 70%;
  margin: auto;
  padding: 250px 0;

  h2 {
    color: #fff;
    font-size: 50px;
    width: 38%;
    font-family: "Playfair Display", serif;
  }
}

.info_junbo {
  color: #fff;
  span {
    color: #fff;
    font-weight: bold;
  }
}

.junboImg {
  background-image: url(../../assets/img/demo-pet-supplies.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}
</style>