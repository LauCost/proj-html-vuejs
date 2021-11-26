<template>
  <div class="category">
    <div
      class="production"
      v-for="production in category"
      :key="production.name"
    >
      <img :src="production.image" alt="" />
      <p>
        {{ production.name }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Catalog",

  data() {
    return {
      category: [
        {
          name: "Bed (1)",
          image: require("../../../assets/img/product-9-300x300.jpg"),
        },
        {
          name: "Food (6)",
          image: require("../../../assets/img/product-3-300x300.jpg"),
        },
        {
          name: "Toys (6)",
          image: require("../../../assets/img/product-2-300x300.jpg"),
        },
        {
          name: "Transport (6)",
          image: require("../../../assets/img/product-4-300x300.jpg"),
        },
      ],
    };
  },
};
</script>


<style lang="scss">
.category {
  display: flex;
  justify-content: center;
  padding-bottom: 70px;
}
.production {
  text-align: center;
  width: 25%;
  margin-right: 10px;

  img {
    width: 100%;
  }

  p {
    margin-top: 15px;
    font-size: 20px;
    font-weight: bold;
  }
}
</style>