<template>
  <div>
    <TitlePanel></TitlePanel>
  </div>
  <div>
    <AbouteMe></AbouteMe>
  </div>
</template>

<script>
// @ is an alias to /src
import TitlePanel from "@/components/TitlePanel.vue";
import AbouteMe from "@/components/AbouteMe.vue";
export default {
  name: "HomeView",
  components: {
    TitlePanel,
    AbouteMe,
  },
};
</script>

<style scoped></style>
