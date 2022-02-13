<template>
  <div id="app">
    <div id="card1">
      <AnimatedCard>
        <img src="./assets/test.webp">
      </AnimatedCard>
    </div>
  </div>
</template>

<script>
import AnimatedCard from './components/AnimatedCard.vue'

export default {
  name: 'App',
  components: {
    AnimatedCard
  }
}
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  #card1 {
    margin: 0vw 30vw;
  }
</style>
