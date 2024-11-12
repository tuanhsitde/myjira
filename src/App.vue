<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <learning-method></learning-method>
  <learning-computed></learning-computed>
</template>

<script>
import LearningMethod from "@/components/LearningMethod.vue";
import LearningComputed from "@/components/LearningComputed.vue";

export default {
  name: "App",
  components: {
    LearningMethod,
    LearningComputed,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
