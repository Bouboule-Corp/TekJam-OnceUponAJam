<template>
  <div id="app">
    <div id="quote">
      <Quote/>
    </div>
    <img id="bg" src="./assets/arrow_bg.png">
    <div id="card" style="top: 85vh; margin: 0vw 5vw;">
      <AnimatedCard number="0">
        <img style="object-fit: contain" src="./assets/1.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 145vh; margin: 0vw 45vw;">
      <AnimatedCard number="1">
        <img style="object-fit: contain" src="./assets/2.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 205vh; margin: 0vw 55vw;">
      <AnimatedCard number="2">
        <img style="object-fit: contain" src="./assets/3.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 265vh; margin: 0vw 35vw;">
      <AnimatedCard number="3">
        <img style="object-fit: contain" src="./assets/4.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 325vh; margin: 0vw 30vw;">
      <AnimatedCard number="4">
        <img style="object-fit: contain" src="./assets/5.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 385vh; margin: 0vw 40vw;">
      <AnimatedCard number="5">
        <img style="object-fit: contain" src="./assets/6.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 445vh; margin: 0vw 30vw;">
      <AnimatedCard  number="6">
        <img style="object-fit: contain" src="./assets/7.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 505vh; margin: 0vw 23vw;">
      <AnimatedCard number="7">
        <img style="object-fit: contain" src="./assets/8.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 565vh; margin: 0vw 15vw;">
      <AnimatedCard number="8">
        <img style="object-fit: contain" src="./assets/9.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 625vh; margin: 0vw 5vw;">
      <AnimatedCard  number="9">
        <img style="object-fit: contain" src="./assets/10.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 685vh; margin: 0vw 15vw;">
      <AnimatedCard  number="10">
        <img style="object-fit: contain" src="./assets/11.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 725vh; margin: 0vw 20vw;">
      <AnimatedCard  number="11">
        <img style="object-fit: contain" src="./assets/12.png">
      </AnimatedCard>
    </div>
    <div id="card" style="top: 750vh; margin: 0vw 25vw;">
      <AnimatedCard  number="12">
        <img style="object-fit: contain" src="./assets/13.png">
      </AnimatedCard>
    </div>
  </div>
</template>

<script>
import Quote from './components/Quote.vue'
import AnimatedCard from './components/AnimatedCard.vue'

export default {
  name: 'App',
  components: {
    Quote,
    AnimatedCard
  }
}
</script>

<style>
  #app {
    font-family: Roboto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    /* text-align: center; */
    color: #2c3e50;
    margin-top: 5px;
  }
  #quote {
    position: absolute;
    margin-top: 25vh;
  }
  #bg {
    position: absolute;
    left: 0;
    max-width: 100%;
    object-fit: contain;
    z-index: -1;
  }
  #bg_bottom {
    position: absolute;
    background-color: red;
    bottom: 0;
    /* height: 40vh;
    width: 100vw; */
  }
  #card {
    position: relative;
  }
</style>
