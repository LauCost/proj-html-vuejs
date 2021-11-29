<template>
  <div class="cont_70 margin_center">
    <div class="cont_links">
      <div class="card_links">
        <img src="../../../assets/img/mobile-light-pet-logo-2x.png" alt="" />
        <p>
          1234 Avada Avenue Avadaville <br />
          info@your-company.com <br />
          Call us:(1) 234 5678
        </p>
      </div>
      <div class="card_links">
        <h3>Shop by brand</h3>
        <ul v-for="infoLink in infoLinks" :key="infoLink.id">
          <li>
            <a href="#">{{ infoLink }}</a>
          </li>
        </ul>
      </div>
      <div class="card_links">
        <h3>Useful links</h3>
        <ul v-for="Link in usefulLikns" :key="Link.id">
          <li>
            <a href="#">{{ Link }}</a>
          </li>
        </ul>
      </div>
      <div class="card_links news_letter_footer">
        <h3>Subscribe to our newsletter</h3>
        <input type="text" placeholder="Insert your email...*" />
        <button>Subscribe</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Links",

  data() {
    return {
      infoLinks: ["Bed", "Food", "Toy", "Transport"],

      usefulLikns: ["My account", "Orders", "Checkout", "Cart"],
    };
  },
};
</script>


<style lang="scss">
.cont_links {
  padding: 100px 0;
  display: flex;
  justify-content: space-between;
  border-bottom: 1px solid #304232;
}

.card_links {
  width: 24%;

  img {
    width: 60%;
  }

  p {
    color: #fff;
  }

  h3 {
    color: #fff;
  }

  ul {
    list-style: none;

    li {
      margin: 20px 0;

      a {
        text-decoration: none;
        color: #fff;
      }
    }
  }
}

.news_letter_footer {
  background-color: #264229;
  background-image: url(../../../assets/img/bg-transparent-3.png);
  display: flex;
  flex-direction: column;
  border-radius: 20px;

  h3 {
    margin: 15px 0;
    margin-left: 40px;
    width: 50%;
  }

  input {
    border: none;
    border-radius: 50px;
    margin: 15px 0;
    margin-left: 40px;
    width: 70%;
    padding: 15px;
    font-weight: bold;
  }

  button {
    border: none;
    width: 70%;
    padding: 15px;
    border-radius: 50px;
    color: #fff;
    background-color: #409ad3;
    font-weight: bold;
    margin: 15px 0;
    margin-left: 40px;
  }
}
</style>