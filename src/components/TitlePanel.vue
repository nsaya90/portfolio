<template>
  <div class="row">
    <div
      class="d-flex flex-column justify-content-center align-items-center box-image"
    >
      <div
        class="d-flex flex-column justify-content-center align-items-center p-4 box-info animate__animated animate__fadeInDownBig"
      >
        <h1 class="text-center">SAYATHAM Nicolas</h1>

        <p class="animate__animated animate__backInLeft">
          Développeur web/mobile
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Afacad:wght@600&family=Lato:wght@300&display=swap");

h1,
p {
  color: white;
  font-family: "Afacad", sans-serif;
}

.animate__animated.animate__backInLeft {
  --animate-duration: 2s;
}

/* -----------------------Mobile */
@media (max-width: 567px) {
  .box-image {
    background-image: url(../assets/images/title_panel.png);

    background-size: cover;
    background-position: center;
    height: 450px;
    width: 100%;
  }

  .box-info {
    border: solid 4px gainsboro;
    height: 225px;
    width: 225px;
  }
  .box-card {
    height: 100%;
  }
}

/* --------------------------DESKTOP */
@media (min-width: 567px) {
  p {
    font-size: 28px;
  }
  .box-image {
    background-image: url(../assets/images/title_panel.png);

    background-size: cover;
    background-position: center;
    height: 920px;
    width: 100%;
  }

  .box-info {
    border: solid 4px gainsboro;
    height: 500px;
    width: 500px;
  }
  .box-card {
    height: 100%;
  }
}
</style>
