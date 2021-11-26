<template>
  <div class="cont_70 flex_center">
    <nav class="flex">
      <div v-for="link in nav" :key="link.name">
        <a
          v-if="
            link.name == 'Home' ||
            link.name == 'Shop' ||
            link.name == 'Shop by brand'
          "
          href="#"
        >
          {{ link.name }} <i class="fas fa-chevron-down"></i>
        </a>
        <a v-else href="#">
          {{ link.name }}
        </a>
      </div>
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

    i {
      font-size: 11px;
      margin-left: 5px;
    }
  }
}

.flex_center {
  display: flex;
  justify-content: center;
}

.flex {
  display: flex;
}

.bold {
  font-weight: bold;
}
</style>