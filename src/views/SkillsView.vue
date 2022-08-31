<template>
  <div class="home">
    <h1 class="color">Skills</h1>
    <h2>Here are some of the "programming" language I can code</h2>
  </div>
  <div class="container">
    <div class="cube">
      <div class="face top">HTML</div>
      <div class="face bottom">Java Script</div>
      <div class="face left">CSS</div>
      <div class="face right">Vue</div>
      <div class="face front">Python</div>
      <div class="face back">Bash</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skills",
};
</script>

<style scoped>
.home {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: column;
  margin: 7% 0 0 1rem;
  text-align: left;
}
h1 {
  font-size: 7rem;
  margin-bottom: -1rem;
}
.color {
  text-shadow: 2px 10px #391153, 4px 5px #ff0000;
}
.container {
  width: 100%;
  height: 100%;
  perspective: 1000px;
  display: flex;
  align-items: center;
  justify-content: center;
}

@keyframes turn {
  0% {
    transform: rotate3d(1, 0, 0, 0deg);
  }

  50% {
    transform: rotate3d(0, 1, 1, 180deg);
  }

  100% {
    transform: rotate3d(1, 1, 1, 360deg);
  }
}

.face {
  width: 200px;
  height: 200px;
  background: rgba(000, 000, 000, 0.4);
  border: 2px solid black;
  position: absolute;
  opacity: 0.5;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: Arial, sans-serif;
  font-size: 2rem;
}
.cube {
  position: relative;
  width: 200px;
  height: 200px;
  transform-style: preserve-3d;
  transform: rotate3d(1, 1, 0, 45deg);
  animation: turn 5s linear infinite;
}
.front {
  transform: translateZ(100px);
}
.back {
  transform: translateZ(-100px) rotateY(180deg);
}
.left {
  transform: translateX(-100px) rotateY(-90deg);
}

.right {
  transform: translateX(100px) rotateY(90deg);
}
.top {
  transform: translateY(-100px) rotateX(90deg);
}

.bottom {
  transform: translateY(100px) rotateX(-90deg);
}
</style>
