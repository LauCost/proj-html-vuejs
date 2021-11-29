<template>
  <div class="cont_social">
    <nav>
      <a v-for="link in links" :key="link" href="#">
        {{ link }}
      </a>
    </nav>
    <p>
      <i class="fab fa-facebook-f"></i>
      <i class="fab fa-twitter"></i>
      <i class="fab fa-instagram"></i>
      <i class="fab fa-youtube"></i>
    </p>
  </div>
</template>

<script>
export default {
  name: "Social",

  data() {
    return {
      links: ["Home", "About", "Blog", "Contact", "Shop"],
    };
  },
};
</script>

<style lang="scss">
.cont_social {
  text-align: center;
  padding: 50px 0 100px 0;

  p {
    color: #fff;

    i {
      margin-top: 50px;
      margin-right: 20px;
      font-size: 20px;
    }
  }
}
</style>