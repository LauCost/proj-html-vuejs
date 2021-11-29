<template>
  <div class="cont_70 margin_auto">
    <div class="info_show">
      <h2>Browse by category</h2>
      <p>
        Augue purus et, tincidunt condimentum mauris. At nibh rutrummi in. Nisi,
        vitae interdum eleifend dui, consequat nulla rhoncus dictum. Viverra.
      </p>
    </div>
    <Catalog />
    <Food />
    <NewWeekly />
    <BestSeller />
  </div>
</template>

<script>
import Catalog from "./Content Show Case/Catalog.vue";
import Food from "./Content Show Case/Food.vue";
import NewWeekly from "./Content Show Case/NewWeekly.vue";
import BestSeller from "./Content Show Case/BestSeller.vue";
export default {
  name: "Showcase",

  components: {
    Catalog,
    Food,
    NewWeekly,
    BestSeller,
  },
};
</script>

<style lang="scss">
.info_show {
  padding: 100px 0;
  h2 {
    text-align: center;
    font-family: "Playfair Display", serif;
    font-size: 30px;
    font-weight: 400;
  }

  p {
    text-align: center;
    width: 35%;
    margin: 20px auto;
  }
}
</style>