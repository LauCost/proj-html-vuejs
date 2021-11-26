<template>
  <header>
    <div class="cont_70 flex_space_between">
      <div class="logo">
        <img src="../assets/img/dark-pet-logo.png" alt="" />
      </div>
      <Search />
    </div>
  </header>
</template>



<script>
import Search from "./Content Header/SearchBar.vue";
export default {
  name: "Header",

  components: {
    Search,
  },
};
</script>




<style lang="scss">
.cont_70 {
  width: 70%;
  margin: 20px auto;
}

.flex_space_between {
  display: flex;
  justify-content: space-between;
}
</style>
