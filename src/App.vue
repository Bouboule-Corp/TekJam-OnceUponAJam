<template>
  <div id="app">
    <Home/>
    <div id="card1">
      <AnimatedCard>
        <img src="./assets/test.webp">
      </AnimatedCard>
    </div>
  </div>
</template>

<script>
import Home from './Home.vue'
import AnimatedCard from './components/AnimatedCard.vue'

export default {
  name: 'App',
  components: {
    Home,
    AnimatedCard
  }
}
</script>

<style>
  #app {
    font-family: Roboto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 5px;
  }
  #bg {
    position: absolute;
  }
  #bg_bottom {
    position: absolute;
    background-color: red;
    bottom: 0;
    /* height: 40vh;
    width: 100vw; */
  }
  #card1 {
    position: relative;
    top: 90vw;
    margin: 0vw 30vw;
  }
</style>
