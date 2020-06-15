<template>
  <div id="app">
    <Resume />
    <Goal />
    <Portfolio />
    <Video />
    <Tip />
  </div>
</template>

<script>
import Resume from "./components/Resume.vue";
import Goal from "./components/Goal.vue";
import Portfolio from "./components/Portfolio.vue";
import Video from "./components/Video.vue";
import Tip from "./components/Tip.vue";

export default {
  name: "App",
  components: {
    Resume,
    Goal,
    Portfolio,
    Video,
    Tip
  }
};
</script>

<style>
#app {
  position: relative;
  background: #f8f8fc;

  width: 375px;
  height: 1956px;

  padding: 24px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
