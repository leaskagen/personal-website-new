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

// AOS is a library for animating elements on scroll
onMounted(() => {
    AOS.init();
})
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');

#app {
  text-align: center;
  font-family: 'Rubik', sans-serif;
  color: #202020;
}

nav {
  padding: 0.5em 1.5em;
  height: 2.75em;
  position: fixed;
  display: flex;
  gap: 1.5em;
  z-index: 100;
  backdrop-filter: blur(5px);
  width: 100%;
  text-align: left;
}

nav a {
  font-size: 1.75em;
  color: #20202080;
}

nav a:hover {
  color: #202020;
}
</style>
