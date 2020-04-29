<template>
  <div id="app">
    <CompositionCounter />
    <BasicCounter />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import CompositionCounter from "./components/Composition-Counter.vue";
import BasicCounter from "./components/Basic-Counter.vue";

export default Vue.extend({
  name: "App",
  components: {
    CompositionCounter,
    BasicCounter,
  },
});
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
