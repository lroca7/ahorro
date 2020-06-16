<template>
  <div id="app">
    <Resume />

    <Goal />

    <Portfolio />

    <Video />

    <Tip />
    <Menu />
  </div>
</template>

<script>
import Resume from "./components/Resume.vue";
import Goal from "./components/Goal.vue";
import Portfolio from "./components/Portfolio.vue";
import Video from "./components/Video.vue";
import Tip from "./components/Tip.vue";
import Menu from "./components/Menu.vue";

export default {
  name: "App",
  components: {
    Resume,
    Goal,
    Portfolio,
    Video,
    Tip,
    Menu
  }
};
</script>

<style>
body {
  background: #f8f8fc;
}
#app {
  position: relative;
  background: #f8f8fc;
  /* background: #d0d0d1; */
  width: 375px;
  height: 1956px;

  padding: 24px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
