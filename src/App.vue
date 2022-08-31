<template>
  <Header />
  <router-view />
</template>

<script>
import Header from "./components/Header.vue";

export default {
  components: {
    Header,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  margin: 0;
  padding: 0;
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: row;
}
body {
  display: flex;
  flex-direction: row;
  margin: 0;
  padding: 0;
  background-color: rgb(33, 33, 33);
  height: 100vh;
  width: 100%;
}
</style>
