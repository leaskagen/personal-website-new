<template>
  <nav>
    <a href="#welcome" data-menuanchor="welcome">Lea Skagen</a>
    <a href="#projects" data-menuanchor="projects">Projects</a>
    <a href="#about" data-menuanchor="about">About me</a>
    <a href="#contact" data-menuanchor="contact">Contact</a>
  </nav>
    <router-view/>
</template>

<script setup>

import { onMounted } from "vue";
import AOS from "aos";

onMounted(() => {
    AOS.init();
})


/*
export default {
  name: 'App',
  function mounted() {
  AOS.init()
}
}
*/
</script>

<style>

@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');

#app {
  /*font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;*/
  font-family: 'Rubik', sans-serif;
  color: #202020;
}

nav {
  padding: 0.5em 1.5em;
  height: 2.75em;
  /*height: 100vh;*/
  position: fixed;
  /*right: 0;*/
  display: flex;
  /*flex-direction: column;*/
  /*justify-content: center;*/
  gap: 1.5em;
  z-index: 100;
  /*text-align: right;*/
  backdrop-filter: blur(5px);
  width: 100%;
  text-align: left;

}

nav a {
  font-size: 1.75em;

  color: #20202080;
  /*width: 100%;*/
}

nav a:hover {
  color: #202020;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
