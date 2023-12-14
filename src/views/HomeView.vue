<template>
  <div>
    <TitlePanel></TitlePanel>
  </div>
  <div>
    <AbouteMe></AbouteMe>
  </div>

  <div><MySkills></MySkills></div>
</template>

<script>
// @ is an alias to /src
import TitlePanel from "@/components/TitlePanel.vue";
import AbouteMe from "@/components/AbouteMe.vue";
import MySkills from "@/components/MySkills.vue";

export default {
  name: "HomeView",
  components: {
    TitlePanel,
    AbouteMe,
    MySkills,
  },
};
</script>

<style scoped></style>
