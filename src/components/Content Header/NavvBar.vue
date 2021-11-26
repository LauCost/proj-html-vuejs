<template>
  <div class="cont_70 flex_center">
    <nav>
      <a v-for="link in nav" :key="link.name" href="#">
        {{ link.name }}
      </a>
    </nav>
  </div>
</template>


<script>
export default {
  name: "NavvBar",

  data() {
    return {
      nav: [
        {
          name: "Home",
        },
        {
          name: "Shop",
        },
        {
          name: "About",
        },
        {
          name: "Blog",
        },
        {
          name: "Contact",
        },
        {
          name: "Shop by brand",
        },
      ],
    };
  },
};
</script>


<style lang="scss">
nav {
  a {
    text-decoration: none;
    margin: 0 15px;
    font-size: 18px;
    color: #adadad;
  }
}

.flex_center {
  display: flex;
  justify-content: center;
}

.bold {
  font-weight: bold;
}
</style>