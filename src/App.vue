<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Main from "./components/Main.vue";
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Main,
    Header,
    Footer,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@300&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Padauk&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Domine&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Source Sans Pro", sans-serif;
}

.cont_70 {
  width: 70%;
}

.margin_auto {
  margin: 20px auto;
}

.margin_center {
  margin: auto;
}

.back_repeat_x {
  background-repeat: repeat-x;
}

.back_green {
  background-color: #1e3120;
  background-image: url(./assets/img/bg-transparent-3.png);
}

.flex {
  display: flex;
  flex-wrap: wrap;
}

.flex_between {
  display: flex;
  justify-content: space-between;
}

.justy_between {
  justify-content: space-between;
}
</style>
