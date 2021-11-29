<template>
  <div class="cont_70 cont_new_production">
    <h2>New products arrival</h2>
    <p class="subtitle_new_production">Latest products</p>
    <div class="flex justy_between">
      <div
        class="card_new_products"
        v-for="newProduction in newProductions"
        :key="newProduction.id"
      >
        <img :src="newProduction.image" alt="" />
        <p class="title_new_production">
          {{ newProduction.title }}
        </p>
        <p class="price" v-if="newProduction.newPrice == '18.00'">
          <span> ${{ newProduction.price }} </span>

          ${{ newProduction.newPrice }}
        </p>
        <p class="price" v-else>${{ newProduction.price }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "NewProduction",

  data() {
    return {
      newProductions: [
        {
          id: 1,
          image: require("../../assets/img/product-8-500x500.jpg"),
          title: "Colored pet bed",
          price: "18.00 - $26.00",
        },
        {
          id: 2,
          image: require("../../assets/img/product-2-500x500.jpg"),
          title: "Colorful ball set",
          price: "29.00",
        },
        {
          id: 3,
          image: require("../../assets/img/product-3-500x500.jpg"),
          title: "Dog bone",
          price: "29.00",
          newPrice: "18.00",
        },
        {
          id: 4,
          image: require("../../assets/img/product-4-500x500.jpg"),
          title: "Animal trasport bag",
          price: "29.00",
        },
        {
          id: 5,
          image: require("../../assets/img/product-5-500x500.jpg"),
          title: "Animal transport cage",
          price: "35.00",
        },
        {
          id: 6,
          image: require("../../assets/img/product-10-500x500.jpg"),
          title: "Closable cat",
          price: "16.00",
        },
      ],
    };
  },
};
</script>


<style lang="scss">
.cont_new_production {
  text-align: center;
  padding-bottom: 70px;

  h2 {
    font-family: "Domine", serif;
    font-size: 45px;
    font-weight: 400;
    padding-top: 80px;
  }

  .subtitle_new_production {
    margin: 30px 0 20px 0;
    color: #2f6c00;
    font-weight: bold;
  }
}

.card_new_products {
  width: 33%;
  margin-top: 70px;
  display: flex;
  flex-direction: column;
  align-items: center;

  img {
    width: 100%;
  }

  .title_new_production {
    font-size: 20px;
    font-weight: bold;
    margin: 25px 0;
  }
}
</style>