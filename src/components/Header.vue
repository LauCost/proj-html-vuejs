<template>
  <header>
    <div class="cont_70 flex_space_between margin_auto">
      <div class="logo">
        <img src="../assets/img/dark-pet-logo.png" alt="" />
      </div>
      <Search />
      <div class="question">
        <p><span>Question?</span> Call us : 1.800.123.4567</p>
      </div>
      <div class="icons">
        <i class="fas fa-shopping-bag"></i>
        <i class="far fa-user"></i>
      </div>
    </div>
    <hr />
    <NavBar />
  </header>
</template>



<script>
import Search from "./Content Header/SearchBar.vue";
import NavBar from "./Content Header/NavvBar.vue";

export default {
  name: "Header",

  components: {
    Search,
    NavBar,
  },
};
</script>




<style lang="scss">
hr {
  border: 1px solid #f9f9f9;
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

.icons {
  i {
    margin-right: 10px;
  }
}
</style>
