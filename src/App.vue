<template>
  <div id="app">
    <Resume />
    <Goal />
    <Portfolio />
  </div>
</template>

<script>
import Resume from "./components/Resume.vue";
import Goal from "./components/Goal.vue";
import Portfolio from "./components/Portfolio.vue";

export default {
  name: "App",
  components: {
    Resume,
    Goal,
    Portfolio
  }
};
</script>

<style>
body {
  background: slategrey;
  padding: 0;
  margin: 0;
}
#app {
  position: relative;
  /* width: 375px; */
  width: 100%;
  height: 1956px;
  background: #f8f8fc;
  padding: 24px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
