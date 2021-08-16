<template>
  <Header />
  <Hero />
  <Content />
</template>

<script>
import Header from "./components/Header"
import Hero from "./components/Hero"
import Content from "./components/Content"

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Content,
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700&display=swap");
@import "@/assets/main.scss";
#app {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
}
</style>
