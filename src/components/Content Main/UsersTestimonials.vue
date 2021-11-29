<template>
  <div class="back_green text_center back_repeat_x">
    <h2>Users testimonials</h2>
    <div class="cont_70 category">
      <div class="testimonial" v-for="user in users" :key="user.id">
        <img :src="user.image" alt="" />
        <p class="text_testimonial">
          {{ user.testiomonial }}
        </p>
        <p class="text_name">{{ user.name }} ThemeFusion</p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "UsersTestimonials",

  data() {
    return {
      users: [
        {
          id: 1,
          image: require("../../assets/img/avatar-3-200x200.jpg"),
          testiomonial:
            "Auctor est habitasse amet nunc, interdum vel mattis sodales cras. Ut nulla quis nunc, tincidunt.eu. Eu.",
          name: "Lisa Smith,",
        },
        {
          id: 2,
          image: require("../../assets/img/avatar-1-200x200.jpg"),
          testiomonial:
            "Donec sollicitudin molestie malesuada. Vivamus suscipit tortor eget falis porttitor volutpat vestibulum ac diam sit.",
          name: "Melissa Green,",
        },
        {
          id: 3,
          image: require("../../assets/img/avatar-4-200x200.jpg"),
          testiomonial:
            "Curabitur arcu erat, accumsan id imperdiet et, porttitor at sem. Proin eget tortor risus vestibulum ante ipsum.",
          name: "Sam Lewis,",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.text_center {
  text-align: center;

  h2 {
    color: #fff;
    padding: 100px 0 50px 0;
    font-size: 45px;
    font-family: "Playfair Display", serif;
  }
}

.testimonial {
  img {
    border-radius: 50%;
    width: 40%;
    margin: 20px 0;
  }
}

.text_testimonial {
  color: #fff;
  width: 265px;
  font-weight: bold;
  margin: 20px 0;
}

.text_name {
  color: #576962;
  font-weight: bold;
  padding-bottom: 150px;
}
</style>