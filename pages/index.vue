<template>
  <div id="app">
    <p><Flip v-bind:value="counter"/></p>
    <button @click="increase">Increase</button>
  </div>
</template>

<script>
import Flip from "~/components/Flip";

export default {
  name: "App",
  components: {
    Flip
  },
  data() {
    return {
      counter: 0
    };
  },
  methods: {
    increase() {
      this.counter++;
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
