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
        <button>Learn more about us</button>
      </div>
    </div>
    <div class="offert">
      <img src="../../assets/img/food-transparent-5-200x112.png" alt="" />

      <p>
        Get $25 OFF your first purchase of our homemade pet food!
        <span>Visit the shop</span>
      </p>
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

.cont_50 {
  width: 50%;
  margin: auto;
  padding: 20px 0;
}

.cont_70_pad {
  width: 70%;
  margin: auto;
  padding: 280px 0;

  h2 {
    color: #fff;
    font-size: 50px;
    width: 38%;
    font-family: "Playfair Display", serif;
    margin: 30px 0;
  }

  p {
    color: #fff;
    font-weight: bold;
    font-size: 13px;
    font-family: "Padauk", sans-serif;
  }

  button {
    border: none;
    padding: 10px 25px;
    border-radius: 50px;
    color: #4c2038;
    font-weight: bold;
  }

  button:hover {
    cursor: pointer;
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
  background-image: url(../../assets/img/banner-5-2x-scaled.jpg);
  background-repeat: no-repeat;
  background-size: cover;
}

.offert {
  width: 50%;
  margin: auto;
  text-align: center;
  padding-top: 15px;
  color: #fff;
  font-size: 20px;
  display: flex;
  align-items: center;

  p {
    margin-left: 20px;
  }
  span {
    margin-left: 20px;
    text-decoration: underline;
    color: #8b9989;
  }
}
</style>