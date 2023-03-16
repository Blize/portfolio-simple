<template>
  <div id="about">
    <div class="fly-in-text" :class="{ hidden: isNotActive }">
      <h1>A</h1>
      <h1>B</h1>
      <h1>O</h1>
      <h1>U</h1>
      <h1>T</h1>
    </div>
    <h2>
      Hey there, I am a 17 years young developer and designer. I live in a
      <br />
      small village in Bern. I am at my second year at swisscom.<br />
      I am an application developer and have experienced many areas of computer
      science.<br />
    </h2>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isNotActive: true,
    };
  },
  mounted() {
    setTimeout(() => {
      this.isNotActive = false;
    }, 250);
  },
};
</script>

<style scoped>
#about {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: column;
  text-align: left;
  margin: 7% 0 0 2rem;
}
.fly-in-text {
  display: flex;
  align-items: flex-start;
  justify-content: flex-start;
  flex-direction: row;
}
.fly-in-text h1 {
  padding: 5px;
  opacity: 1;
  transition: all 1.3s ease;
}
.fly-in-text.hidden h1 {
  opacity: 0;
}
.fly-in-text.hidden h1:nth-child(1) {
  transform: translateX(-400px) translateY(-200px);
}
.fly-in-text.hidden h1:nth-child(2) {
  transform: translateX(20px) translateY(100px);
}
.fly-in-text.hidden h1:nth-child(3) {
  transform: translateX(-150px) translateY(-80px);
}
.fly-in-text.hidden h1:nth-child(4) {
  transform: translateX(10px) translateY(-200px);
}
.fly-in-text.hidden h1:nth-child(5) {
  transform: translateX(-300px) translateY(200px);
}
.fly-in-text.hidden h1:nth-child(6) {
  transform: translateX(20px) translateY(-20px);
}
.fly-in-text.hidden h1:nth-child(7) {
  transform: translateX(50px) translateY(250px);
}
h1 {
  font-size: 7rem;
  text-shadow: 2px 10px #391153, 4px 5px #ff0000;
  margin-bottom: -1rem;
}
h1:hover {
  scale: 0.9;
  transform: rotateY(30deg);
  transition-duration: 0.2s;
}

h2 {
  font-weight: 200;
}
</style>
