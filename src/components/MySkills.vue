<template>
  <div class="box-skills">
    <div class="box-skills-web">
      <div class="box">
        <div class="box-web">
          <h2 :class="animate_1">
            <i class="fa-solid fa-code"></i> Compétences techniques
          </h2>
          <ul :class="animate_2">
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
          <h2 :class="animate_3">
            <i class="fa-regular fa-user"></i> Savoir-être
          </h2>
          <ul :class="animate_4">
            <li>Rigoureux</li>
            <li>Autonome</li>
            <li>Organisé</li>
            <li>Esprit d'équipe</li>
          </ul>
        </div>
      </div>
      <div :class="animate_5">
        <img src="../assets/cv.png" class="cv" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scrollPosition: 0,
      targetElementOffset: 1000, // Ajoutez la valeur de l'offset de l'élément cible ici
      condition: false,
    };
  },
  methods: {
    handleScroll() {
      // Mettre à jour la position de défilement actuelle
      this.scrollPosition = window.scrollY;

      // Vérifier si l'utilisateur a atteint l'endroit souhaité
      if (this.scrollPosition >= this.targetElementOffset) {
        // L'utilisateur a atteint l'endroit souhaité
        this.condition = true; // Vous pouvez effectuer des actions supplémentaires ici
      }
    },
  },
  computed: {
    animate_1() {
      return { "animate__animated animate__zoomIn": this.condition };
    },
    animate_2(){
      return { "animate__animated animate__lightSpeedInRight" : this.condition}
    },
    animate_3(){
      return{ "animate__animated animate__zoomIn": this.condition}
    },
    animate_4(){
      return { "animate__animated animate__lightSpeedInLeft" : this.condition}
    },
    animate_5(){
      return { "animate__animated animate__fadeIn" : this.condition}
    }
  },
  mounted() {
    // Ajouter un gestionnaire d'événement de défilement
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeUnmount() {
    // Supprimer le gestionnaire d'événement de défilement lors de la destruction du composant
    window.removeEventListener("scroll", this.handleScroll);
  },
};
</script>


<style scoped>
.animate__animated.animate__zoomIn, .animate__animated.animate__lightSpeedInLeft, .animate__animated.animate__lightSpeedInRight , .animate__animated.animate__fadeIn {
  --animate-duration: 3s;
}
.test {
  background-color: red;
}
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
    width: 25%;
  }
  .box-skills {
    display: flex;
    justify-content: space-between;
    width: 100%;
  
  }

  .box-skills-web {
    display: flex;
    justify-content: space-between;
    width: 100%;
    padding-top: 25px;
  }
}
</style>
