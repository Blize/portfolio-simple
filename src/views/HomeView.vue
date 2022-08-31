<template>
  <div class="home">
    <h1>Hi,</h1>
    <h1 class="under-title">
      I'm
      <span class="color">Matthias</span>
    </h1>
    <h2 class="animation">Developer, Designer and Human</h2>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeView",
  components: {},
});
</script>

<style scoped>
.home {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: column;
  margin: 7% 0 0 1rem;
}
h1 {
  font-size: 7rem;

  margin-bottom: -1rem;
}
.color {
  text-shadow: 2px 10px #391153, 4px 5px #ff0000;
}
.under-title {
  margin-top: -2rem;
}
.animation {
  animation: fadeIn 2s;
}
@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  60% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
