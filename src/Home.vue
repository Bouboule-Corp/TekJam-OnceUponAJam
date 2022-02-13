<template>
  <div>
    <div class="marquee-rtl">
      <div>
        {{quotes}}
      </div>
      <hr class="solid" />
    </div>
  </div>
</template>

<script>

export default {
  name: "Home",

  data() {
    return {
      quotes: "Avoir un grain de folie c'est aimer la vie, pas être bourré BÉBÉ ! (Sébastien Soriano) • N'essayez pas de devenir un homme qui a du succès. Essayez de devenir un homme qui a de la valeur. (Albert Einstein) • Soit A un succès dans la vie. Alors A = x + y + z, où x = travailler, y = s'amuser, z = se taire. (Albert Einstein) • Aucun de nous, en agissant seul, ne peut atteindre le succès. (Nelson Mandela) • Le succès est un mauvais professeur. Il pousse les gens intelligents à croire qu'ils sont infaillibles. (Bill Gates) • Le succès ne s'imite pas, il se crée. (Luis Fernandez) • Le succès c'est d'aller d'échec en échec sans perdre son enthousiasme. (Winston Churchill) • La déception est bien moins pénible quand on ne s'est point d'avance promis le succès. (Sénèque) • Le succès n'a pas besoin d'explication, l'échec n'admet pas de justification. (Luis Fernandez) • Un succès orthographié insuccès vire à l'échec. (Gilbert Choulet) • La jalousie des autres peintres a toujours été le thermomètre de mon succès. (Salvador Dali) • Le grand succès des ennemis de l'Afrique, c'est d'avoir corrompu les Africains eux-mêmes. (Frantz Fanon) • La chance d'un homme, le succès d'un homme, la paix d'un homme, c'est le bon comportement. (Mohamed Cherif) • N'importe qui peut sympathiser avec les souffrances d'un ami. Sympathiser avec ses succès exige une nature très délicate. (Oscar Wilde) • La formation est l'essence de tout succès. (Arnaud Boti) • Pour que votre voyage de noces soit un succès total sur le plan touristique, sentimental et sexuel, la première chose à faire est de partir seul. (Pierre Desproges) • Pour connaître les amis il est nécessaire de passer par le succès et le malheur. Dans le succès, nous vérifions la quantité et dans le malheur la qualité. (Confucius) • Le succès est le résultat d'une succession d'échecs que l'on a surmonté sans jamais abandonner. (Adrien Verschaere) • Le succès, ça rend modeste quand t'es pas trop con. Et grâce à lui, tu rencontres des tas de surdoués qui n'y accèdent jamais. (Coluche) • Cette philosophie [japonaise], qui est une des raisons principales de leur succès, n'a pu se maintenir comme principe d'existence du peuple que parce que celui-ci est resté protégé contre le poison du christianisme. Comme dans l'Islam, la religion japonaise est dépourvue de tout terrorisme et contient seulement l'espoir de la félicité. Le terrorisme est seulement une idée juive répandue par le christianisme. (Adolf Hitler)",
    };
  },
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
  animation: defilement-rtl 200s infinite linear; /* défilement */
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
