<template>
  <div class="cont_love">
    <p>All-time best sellers</p>
    <div class="flex_space_between">
      <h2>Items everyone loves</h2>
      <button>View all products</button>
    </div>
    <div class="flex_space_between">
      <div
        class="card_best"
        v-for="production in productions"
        :key="production.name"
      >
        <img :src="production.image" alt="" />
        <p class="name_production">
          {{ production.name }}
        </p>
        <p class="price" v-if="production.price == '35.00'">
          <span> $ {{ production.price }} </span>
          ${{ production.discounted }}
        </p>
        <p class="price" v-else>$ {{ production.price }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BestSeller",

  data() {
    return {
      productions: [
        {
          name: "Transport cage",
          price: "25.00",
          image: require("../../../assets/img/product-21-400x400.jpg"),
        },
        {
          name: "Dog leash",
          price: "25.00",
          image: require("../../../assets/img/product-20-400x400.jpg"),
        },
        {
          name: "Animal transport cage",
          price: "35.00",
          discounted: "25.00",
          image: require("../../../assets/img/product-16-400x400.jpg"),
        },
        {
          name: "Colorful cat leash",
          price: "12.00",
          image: require("../../../assets/img/product-11-400x400.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.cont_love {
  margin: 100px 0;

  h2 {
    font-family: "Playfair Display", serif;
    font-weight: 400;
    font-size: 40px;
  }

  p {
    color: #2f6c00;
    font-weight: bold;
    margin-bottom: 20px;
  }
  button {
    border: none;
    padding: 15px 35px;
    border-radius: 50px;
    color: #fff;
    background-color: #409ad3;
    font-weight: bold;
  }

  button:hover {
    cursor: pointer;
  }
}

.card_best {
  width: 24%;
  margin-top: 70px;
  display: flex;
  flex-direction: column;
  align-items: center;

  img {
    width: 100%;
  }

  .name_production {
    color: #000000;
    margin-top: 20px;
  }
}

.price {
  font-size: 18px;
  color: #2f6c00;

  span {
    font-size: 15px;
    margin-right: 10px;
    text-decoration: line-through;
  }
}
</style>