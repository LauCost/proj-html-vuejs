<template>
  <div class="copyright">
    <p>
      <i class="far fa-copyright"></i>
      Copyright 2012 | Avada Theme by ThemeFusion | All Rights Reserved |
      Powered by Lori
    </p>
    <div class="up" @click="topFunction()">
      <i class="fas fa-angle-up"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "Copyright",

  methods: {
    topFunction() {
      /* console.log("Click"); */
      document.body.scrollTop = 0;
      document.documentElement.scrollTop = 0;
    },
  },
};
</script>


<style lang="scss">
.copyright {
  background-color: #000;
  text-align: center;
  position: relative;

  p {
    color: #fff;
    padding: 20px 0;
  }

  .up {
    position: absolute;
    background-color: #2e2e2e;
    color: #fff;
    width: 50px;
    height: 40px;
    line-height: 40px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;
    bottom: 0;
    right: 1%;
    transform: translate(-99%, 0);
  }

  .up:hover {
    cursor: pointer;
  }
}
</style>