<template>
  <div id="app">
    <h1>Vue Tag Cloud</h1>
    <p>A jQCloud insipred tag cloud for Vuejs</p>
    <VueTagCloud v-bind:data="tagData"></VueTagCloud>
  </div>
</template>

<script>
import VueTagCloud from "./components/VueTagCloud";

export default {
  name: "app",
  data() {
    return {
      tagData: [
        { text: "Lorem", weight: 15, link: "https://google.com" },
        { text: "Ipsum", weight: 9 },
        { text: "Dolor", weight: 6 },
        { text: "Sit", weight: 7 },
        { text: "Amet", weight: 5 }
      ]
    };
  },
  components: {
    VueTagCloud
  }
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
