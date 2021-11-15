<template>
<div>
 <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0">
  <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700" rel="stylesheet">
  <section class="hero-section">
  <div class="card-grid">
    <a class="card" href="http://47.103.26.126">
      <div class="card__background" :style="delivery"></div>
      <div class="card__content">
        <p class="card__category">Nusist_Dev</p>
        <h3 class="card__heading">南信大校园代拿</h3>
      </div>
    </a>
    <a class="card" @click="click" >
      <div class="card__background" :style="learning"></div>
      <div class="card__content">
        <p class="card__category">Nusist_Dev</p>
        <h3 class="card__heading">学习资料</h3>
      </div>
    </a>
    <!-- <a class="card" href="#">
      <div class="card__background" style="background-image: url(https://images.unsplash.com/photo-1556680262-9990363a3e6d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60)"></div>
      <div class="card__content">
        <p class="card__category">Category</p>
        <h3 class="card__heading">Example Card Heading</h3>
      </div>
    </li> -->
    <a class="card" @click="setClick">
      <div class="card__background" :style="setting"></div>
      <div class="card__content">
        <p class="card__category">Nusist_Dev</p>
        <h3 class="card__heading">更多服务</h3>
      </div>
    </a>
  </div>
</section>
</div>
</template>

<script>
import { Toast } from 'vant';
export default {
  data() {
    return {
      delivery: {
        backgroundImage: "url(" + require("./assets/delivery.jpg") + ")",
      },
      learning: {
        backgroundImage: "url(" + require("./assets/learning.jpg") + ")",
      },
      setting: {
        backgroundImage: "url(" + require("./assets/setting.jpg") + ")",
      },
    }
  },
  name: 'App',
  components: {
  },
  methods: {
    click() {
      Toast('预计11月20号开放改功能');
    },
    setClick() {
      Toast('更多功能，敬请期待~');
    },
  }
}
</script>

<style>
@import './style.css';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
