<template>
  <div>
    <img src="./assets/once-upon-a-tome-de-savoie.png" />
    <div class="marquee-rtl">
      <div>
        Texte défilant horizontalement que la fenêtre de
        défilement
      </div>
      <hr class="solid" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style>
/* Solid border */
hr.solid {
  border-top: 3px solid #bbb;
  margin : 50px
}
/* ---------------------------- */
/* Défilement de droite à gauche */
.marquee-rtl {
  overflow: hidden; /* important */
  width: 100%;
  margin-top: 50px;
}
.marquee-rtl > div {
  display: inline-block; /* important */
  white-space: nowrap; /* important */
  animation: defilement-rtl 20s infinite linear; /* défilement */
  cursor: pointer;
  padding: 10px 2em 10px 100%;
}
.marquee-rtl:hover > div {
  animation-play-state: paused; /* met en pause le défilement */
}
@keyframes defilement-rtl {
  0% {
    -webkit-transform: translate(0);
    transform: translate(0);
  }
  100% {
    -webkit-transform: translate(-100%);
    transform: translate(-100%);
  }
}
/* ---------------------------- */
/* déco */
h2,
p {
  text-align: center;
}

.marquee-rtl > div {
  font-size: 3em;
}

.title {
  font-size: 5em;
}
</style>
