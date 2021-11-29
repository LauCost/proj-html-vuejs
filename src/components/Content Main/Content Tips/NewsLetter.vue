<template>
  <div class="cont_70 back_news">
    <h2>Join our newsletter</h2>
    <p>
      Volutpat vel turpis nulla lorem sed semper. Aliquam sagittis sem libero
      viverra vehicula nullam ut nisl.
    </p>
    <input type="text" placeholder="Insert your email ...*" />
    <button class="sub">Subscribe</button>
  </div>
</template>






<style lang="scss">
.back_news {
  background-image: url(../../../assets/img/banner-7-2x-scaled.jpg);
  padding: 80px 0;
  background-size: cover;
  position: absolute;
  top: -110px;
  left: 50%;
  transform: translate(-50%, 0);
  filter: drop-shadow(1px 1px 1px #fbfaf8);

  h2 {
    font-family: "Domine", serif;
    font-size: 45px;
    font-weight: 400;
    margin: 20px 50px;
  }

  p {
    width: 33%;
    font-weight: bold;
    margin: 20px 50px;
  }

  input {
    width: 25%;
    padding: 16px 13px;
    border-radius: 50px;
    border: none;
    background-color: #f8f5f2;
    margin: 20px 20px 90px 50px;
    color: #000;
    font-weight: bold;
  }
}
.sub {
  border: none;
  padding: 15px 55px;
  border-radius: 50px;
  color: #fff;
  background-color: #409ad3;
  font-weight: bold;
}

.sub:hover {
  cursor: pointer;
}
</style>