<template>
  <div class="box-skills">
    <div class="box-my-skills">
      <h1>Compétences</h1>
      <p>
        Elles sont en constantes améliorations car pour moi la joie de ce métier
        fait que l'on en apprend tous les jours, d'autant plus en étant
        impliqué, curieux et passionné.
      </p>
    </div>

    <div class="box-skills-web">
      <div class="box-web">
        <h2>Développement Web</h2>
        <ul>
          <li>PHP</li>
          <li>MySQL</li>
          <li>Laravel</li>
          <li>Javascript</li>
          <li>VueJS</li>
        </ul>
      </div>
      <div class="box-database">
        <h2>Base de donnée</h2>
        <ul>
          <li>MySQL</li>
          <li>PDO</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.box-skills {
  background-color: #e8f1f2;
}

/* ----------------Mobile------------------ */
@media (max-width: 567px) {
  h1 {
    text-align: center;
    padding-top: 15px;
  }

  p {
    padding: 10px;
    text-align: center;
  }

  li {
    list-style-type: square;
  }
  .box-my-skills {
    display: flex;
    flex-direction: column;
    align-items: center;
   
    
  }
  .box-skills-web {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5px;
  }

  .box-web ,.box-database {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 15px;
    background-color: white;
    border-radius: 10% 10% 10% ;
    width: 80%;
    margin: 25px;
  }

  .box-web h2 , .box-database h2 {
    background-color: #f9f5e3;
    padding: 15px;
    border-top-right-radius: 60px;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 60px;
    border-bottom-right-radius: 20px;
    height: 65px;
  }
}
</style>
