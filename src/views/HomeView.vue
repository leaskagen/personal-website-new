<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<style>
body {
  background: linear-gradient(297deg, #ff6cbe, #f97e99, #dd98fd);
    background-size: 600% 600%;

    -webkit-animation: backgroundAnimation 59s ease infinite;
    -moz-animation: backgroundAnimation 59s ease infinite;
    animation: backgroundAnimation 59s ease infinite;
}

@-webkit-keyframes backgroundAnimation {
    0%{background-position:0% 15%}
    50%{background-position:100% 86%}
    100%{background-position:0% 15%}
}
@-moz-keyframes backgroundAnimation {
    0%{background-position:0% 15%}
    50%{background-position:100% 86%}
    100%{background-position:0% 15%}
}
@keyframes backgroundAnimation {
    0%{background-position:0% 15%}
    50%{background-position:100% 86%}
    100%{background-position:0% 15%}
}

</style>


<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld
  }
}
</script>
