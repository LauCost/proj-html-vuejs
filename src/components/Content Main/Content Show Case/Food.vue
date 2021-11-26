<template>
  <div class="category">
    <div class="card_fod" v-for="food in foods" :key="food.name">
      <h2>
        {{ food.name }}
      </h2>
      <p>
        {{ food.description }}
      </p>
      <div class="food_img">
        <img :src="food.image" alt="" />
      </div>
      <button>Shop {{ food.type }} food</button>
    </div>
  </div>
</template>


<script>
export default {
  name: "Food",

  data() {
    return {
      foods: [
        {
          name: "Kibble",
          description: "Dry dog food",
          image: require("../../../assets/img/food-transparent-18.png"),
          type: "dry",
        },
        {
          name: "Moist",
          description: "Canned dog food",
          image: require("../../../assets/img/food-transparent-17.png"),
          type: "moist",
        },
        {
          name: "Frozen",
          description: "Freeze-Dried dog food",
          image: require("../../../assets/img/food-transparent-16.png"),
          type: "frozen",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.card_fod {
  width: 33%;
  background-color: #1e3120;
  background-image: url(../../../assets/img/bg-transparent-3.png);
  background-position: top;
  background-repeat: repeat-x;
  display: flex;
  flex-direction: column;
  align-items: center;

  h2 {
    color: #fff;
    margin-bottom: 20px;
    padding-top: 70px;
    font-family: "Playfair Display", serif;
    font-size: 35px;
    font-weight: 400;
  }

  p {
    font-size: 20px;
    color: #3b6741;
    font-weight: bold;
  }

  button {
    border: none;
    padding: 15px 35px;
    border-radius: 50px;
    color: #fff;
    background-color: #409ad3;
    margin-bottom: 70px;
    font-weight: bold;
  }

  button:hover {
    cursor: pointer;
  }
}

.food_img {
  width: 50%;
  margin: auto;
  padding: 30px 0;

  img {
    width: 100%;
  }
}
</style>