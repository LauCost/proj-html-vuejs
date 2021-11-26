<template>
  <div class="weekly_back">
    <div class="text_weekly">
      <p>FIND THE BEST ANIMAL SUPPLIES</p>
      <h2>New arrivals weekly</h2>
      <button>Learn more about us</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "NewWeekly",
};
</script>

<style lang="scss">
.weekly_back {
  background-image: url(../../../assets/img/banner-3-2x-scaled.jpg);
  background-size: cover;

  .text_weekly {
    padding: 200px 0;
    margin: auto;
    text-align: center;

    h2 {
      color: #fff;
      font-size: 50px;
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
      padding: 10px 35px;
      border-radius: 50px;
      color: #4c2038;
      font-weight: bold;
    }

    button:hover {
      cursor: pointer;
    }
  }
}
</style>