<template>
  <div class="home">
    <app-navigation></app-navigation>
    <div class="showcaseDiv">
      <h2>The trivia game where millennials go head to head with baby boomers</h2>
      <p>Players answer ten questions to see which side will win!</p>
    </div>
    <div class="homeImages">
      <h2 class="chooseH2">Choose Your Side</h2>
      <div class="homeImage">
        <router-link to="/register">
          <img src="@/assets/millennial.png" alt="millennial" />
          <h2 class="millennialFont">Millennial</h2>
        </router-link>
      </div>
      <div class="homeImage">
        <router-link to="/register">
          <img src="@/assets/boomer.png" alt="boomer" />
          <h2 class="boomerFont">BOOMER</h2>
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from './Navigation.vue'
export default {
  name: 'Home',
  data () {
    return {
    }
  },
  components: {
    'app-navigation': Navigation
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home {
  text-align: center;
}
.welcomeDiv {
  background-color: #388e3c;
  color: white;
}
.showcaseDiv h2{
  margin-top: 50px;
}
.showcaseDiv p {
  margin-top: 20px;
  margin-bottom: 50px;
}
.homeImages {
  width: 100%;
  background-color: #388e3c;
  color: white;
}
.homeImage {
  width: 45%;
  display: inline-block;
}
.chooseH2 {
  font-size: 32px;
  padding-top: 20px;
  padding-bottom: 20px;
}
.homeImage img {
  width: 70%;
}
.homeButton {
  text-align: right;
}
</style>
