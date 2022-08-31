<template>
  <nav>
    <router-link to="/" class="direction">Home</router-link>
    <router-link to="/about" class="direction">About</router-link>
    <router-link to="/skills" class="direction">Skills</router-link>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Header",
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
nav {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: column;
  max-width: 77px;
  border-right: 1px solid rgb(28, 28, 28);
  border-radius: 4px;
  background-color: rgb(28, 28, 28);
  width: fit-content;
  min-height: 100%;
  padding: 1rem;
  margin: 0;
}
.direction {
  margin-top: 1rem;
  font-size: 1rem;
  text-decoration: none;
  color: white;
  position: relative;
  top: 20%;
  padding: 0.5rem;
  transition-duration: 0.5s;
}
.direction:hover {
  transition-duration: 0.5s;
  background-color: gray;
  padding: 0.5rem;
  border-radius: 6px;
}
.direction:active {
  scale: 0.95;
}
</style>
