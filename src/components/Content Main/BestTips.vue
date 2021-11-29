<template>
  <div class="position">
    <NewsLetter />
    <div class="cont_70 padding margin_auto">
      <h2>Get the best tips & tricks</h2>
      <p class="sub_title">Recent articles</p>
      <div class="flex_space_between">
        <div class="card_article" v-for="article in articles" :key="article.id">
          <img :src="article.image" alt="" />
          <h3>
            {{ article.title }}
          </h3>
          <p>
            {{ article.date }}
          </p>
        </div>
      </div>
      <button>Read all articles</button>
    </div>
  </div>
</template>

<script>
import NewsLetter from "./Content Tips/NewsLetter.vue";
export default {
  name: "BestTips",

  components: {
    NewsLetter,
  },

  data() {
    return {
      articles: [
        {
          id: 1,
          image: require("../../assets/img/blog-1-400x400.jpg"),
          title: "How to 'loose leash walk' your dog",
          date: "April 21st, 2020",
        },
        {
          id: 2,
          image: require("../../assets/img/blog-2-400x400.jpg"),
          title: "Stop cats from scratching furniture",
          date: "April 19th, 2020",
        },
        {
          id: 3,
          image: require("../../assets/img/blog-3-400x400.jpg"),
          title: "Where to buy the best pet food",
          date: "April 18th, 2020",
        },
        {
          id: 4,
          image: require("../../assets/img/blog-4-400x400.jpg"),
          title: "Proper care for your pet toys",
          date: "April 17th, 2020",
        },
      ],
    };
  },
};
</script>




<style lang="scss">
.position {
  position: relative;
}

.padding {
  padding-top: 500px;
  display: flex;
  flex-direction: column;
  align-items: center;

  h2 {
    font-size: 35px;
    font-weight: 400;
    font-family: "Domine", serif;
    margin-bottom: 20px;
    text-align: center;
  }

  .sub_title {
    color: #6e916e;
    font-weight: bold;
    text-align: center;
    margin-bottom: 50px;
  }

  button {
    border: none;
    padding: 15px 55px;
    border-radius: 50px;
    color: #fff;
    background-color: #409ad3;
    font-weight: bold;
    margin: 50px 0 100px 0;
  }

  button:hover {
    cursor: pointer;
  }
}

.card_article {
  width: 23%;

  img {
    width: 100%;
  }

  h3 {
    width: 180px;
    margin: 25px 0 15px 45px;
  }

  p {
    margin: 0 0 15px 45px;
    font-weight: bold;
    color: #b9b4b6;
  }
}
</style>