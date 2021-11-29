<template>
  <div class="flex">
    <div class="card_utility" v-for="utility in utilitys" :key="utility.id">
      <img :src="utility.image" alt="" />
      <div class="test">
        <p>
          {{ utility.text }}
        </p>
        <h2>
          {{ utility.title }}
        </h2>
        <button>
          {{ utility.txtButton }}
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "UtilityProduction",

  data() {
    return {
      utilitys: [
        {
          id: 1,
          image: require("../../../assets/img/banner-8-2x.jpg"),
          text: "FINDE THE BEST ANIMAL SUPPLIES",
          title: "Popular accessories",
          txtButton: "View all toys accessories",
        },
        {
          id: 2,
          image: require("../../../assets/img/banner-9-2x.jpg"),
          text: "FIND THE BEST FOOD",
          title: "New Food Arrival",
          txtButton: "View all food products",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.card_utility {
  width: 50%;
  position: relative;

  img {
    width: 100%;
    filter: opacity(0.9);
  }

  .test {
    position: absolute;
    top: 45%;
    left: 50%;
    transform: translate(-50%, -55%);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    height: 30%;

    p {
      color: #fff;
      font-weight: bold;
    }

    h2 {
      color: #fff;
      font-size: 45px;
      font-family: "Domine", serif;
      font-weight: 400;
    }

    button {
      border: none;
      padding: 10px 25px;
      border-radius: 50px;
      color: #4c2038;
      font-weight: bold;
    }
  }
}
</style>