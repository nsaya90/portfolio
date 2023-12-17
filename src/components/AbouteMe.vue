<template>
  <div><h1>A PROPOS DE MOI</h1></div>

  <div class="box-about-me">
    <div class="box-text-about-me">
      <p>
        Je suis ravi de partager avec vous une étape passionnante de ma carrière
        professionnelle. Après avoir consacré une décennie enrichissante au
        domaine de la logistique, je me lance dans une nouvelle aventure en tant
        que développeur web. Ma transition vers le développement web découle de
        ma passion pour la résolution de problèmes et ma fascination pour le
        potentiel infini de la technologie. Mes années dans la logistique m'ont
        apporté rigueur, autonomie ainsi que le travail d'équipe pour être le
        plus efficace possbile. Ces compétences, combinées à mon désir
        d'apprendre et de m'adapter, sont des atouts que je compte mettre à
        profit dans le domaine du développement web.
      </p>
    </div>
    <div class="">
      <img
        src="../assets/images/portrait.jpg"
        alt=""
        height="150"
        width="150" />
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
h1 {
  text-align: center;
  padding-top: 15px;
}

@import url("https://fonts.googleapis.com/css2?family=Afacad:wght@400&family=Lato:wght@300&display=swap");

h1 {
  font-family: "Afacad", sans-serif;
}
p {
  font-family: "Afacad", sans-serif;
  font-size: 25px;
}

/* -----------------------Mobile -----------*/
@media (max-width: 567px) {
  .box-about-me {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    padding: 25px;
  }

  .box-text-about-me {
    padding: 10px;
   
  }
}

/* ----------- DESKTOP --------------- */
@media (min-width: 567px) {
  .box-about-me {
    display: flex;
    justify-content: space-around;
    align-items: center;
  }

  .box-text-about-me {
    padding-top: 25px;
    width: 40%;
  }
}
</style>
