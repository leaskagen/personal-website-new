<template>
  <nav>
    <a href="#welcome" data-menuanchor="welcome">Lea Skagen</a>
    <a href="#projects" data-menuanchor="projects">Projects</a>
    <a href="#contact" data-menuanchor="contact">Contact</a>
  </nav>
  <router-view/>
</template>

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
  padding: 30px;
  height: 100vh;
  position: fixed;
  display: flex;
  flex-direction: column;
  justify-content: center;
  z-index: 100;

}

nav a {
  font-weight: bold;
  color: #2c3e50;
  width: 100%;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
