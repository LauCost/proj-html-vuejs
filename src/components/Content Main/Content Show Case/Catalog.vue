<template>
  <div class="flex">
    <div class="category" v-for="production in category" :key="production.name">
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
          image: require("../../../assets/img/product-9-400x400.jpg"),
        },
        {
          name: "Food (6)",
          image: require("../../../assets/img/product-3-400x400.jpg"),
        },
        {
          name: "Toys (6)",
          image: require("../../../assets/img/product-2-400x400.jpg"),
        },
        {
          name: "Transport (6)",
          image: require("../../../assets/img/product-4-400x400.jpg"),
        },
      ],
    };
  },
};
</script>


<style lang="scss">
.category {
  margin-right: 10px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  p {
    margin-top: 15px;
    font-size: 20px;
    font-weight: bold;
  }
}
</style>