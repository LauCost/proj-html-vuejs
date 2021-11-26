<template>
  <header>
    <div class="cont_70 flex_space_between">
      <div class="logo">
        <img src="../assets/img/dark-pet-logo.png" alt="" />
      </div>
      <Search />
      <div class="question">
        <p><span>Question?</span> Call us : 1.800.123.4567</p>
      </div>
      <div class="icons">
        <i class="far fa-user"></i>
      </div>
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
  align-items: center;
}

.question {
  p {
    font-size: 18px;
    color: black;
  }

  span {
    font-weight: bold;
  }
}
</style>
