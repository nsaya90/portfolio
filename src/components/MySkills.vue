<template>
  <div class="box-skills">
    <div class="box-skills-web">
      <div class="box">
        <div class="box-web">
          <h2 class="animate__animated animate__zoomIn">
            <i class="fa-solid fa-code"></i> Compétences techniques
          </h2>
          <ul class="animate__animated animate__lightSpeedInRight">
            <li>PHP</li>
            <li>MySQL</li>
            <li>Laravel</li>
            <li>Javascript</li>
            <li>VueJS</li>
            <li>MySQL</li>
            <li>Git</li>
          </ul>
        </div>
        <div class="soft-skills">
          <h2 class="animate__animated animate__zoomIn">
            <i class="fa-regular fa-user"></i> Savoir-être
          </h2>
          <ul class="animate__animated animate__lightSpeedInLeft">
            <li>Rigoureux</li>
            <li>Autonome</li>
            <li>Organisé</li>
            <li>Esprit d'équipe</li>
          </ul>
        </div>
      </div>
      <div class="box-cv animate__animated animate__fadeIn">
        <img src="../assets/cv.png" class="cv" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.box-my-skills {
  background-color: rgba(17, 172, 224, 0.989);
  color: white;
  margin-top: 15px;
}
.box-skills {
  background-color: rgb(235, 233, 233);
}
/* ----------------Mobile------------------ */
@media (max-width: 567px) {
  .box-skills {
    background-color: rgb(235, 233, 233);
  }
  i {
    color: rgba(17, 172, 224, 0.989);
  }
  h1 {
    text-align: center;
    padding-top: 15px;
  }

  h2 {
    text-align: center;
  }

  p {
    padding: 10px;
    text-align: center;
  }
  .cv {
    height: 600px;
    width: 100%;
  }

  .box-web li {
    list-style-type: none;
    text-align: center;
    background-color: rgba(17, 172, 224, 0.989);
    margin: 7px;
    padding: 8px;
    border-radius: 7px;
    color: white;
    display: inline-block;
  }

  .soft-skills li {
    list-style-type: none;
    text-align: center;
    background-color: rgb(255, 111, 0);
    margin: 7px;
    padding: 8px;
    border-radius: 7px;
    color: white;
    display: inline-block;
  }

  ul {
    display: block;
    list-style-type: disc;
  }
  .box-my-skills {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .box-skills-web,
  .soft-skills {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5px;
  }

  .box-web {
    padding: 15px;
  }
}

/* --------------------- DESKTOP --------------- */
@media (min-width: 567px) {
  i {
    color: rgba(17, 172, 224, 0.989);
  }
  h1 {
    text-align: center;
    padding-top: 15px;
  }

  h2 {
    text-align: center;
  }

  p {
    padding: 10px;
    text-align: center;
  }
  .cv {
    height: 900px;
    width: 650px;
  }
  .box {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .box-web li {
    list-style-type: none;
    text-align: center;
    background-color: rgba(17, 172, 224, 0.989);
    margin: 7px;
    padding: 8px;
    border-radius: 7px;
    color: white;
    display: inline-block;
    width: 25%;
  }

  .soft-skills li {
    text-align: center;
    background-color: rgb(255, 111, 0);
    margin: 7px;
    padding: 8px;
    border-radius: 7px;
    color: white;
    list-style-type: none;
    display: inline-block;
  }
  .box-skills {
    display: flex;
    justify-content: space-around;
    width: 100%;
    padding: 15px;
  }

  .box-skills-web {
    display: flex;
    justify-content: space-around;
  }
}
</style>
