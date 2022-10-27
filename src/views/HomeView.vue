

<template>
  <div class="home">
    <HomeSection1/>
    <HomeSection2/>
    <HomeSection3/>
    <FooterHome/>
  </div>
</template>

<style>
body {
  background: linear-gradient(297deg, #ffa364, #f97ebe, #dd98fd);

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

import HomeSection1 from '../components/HomeSection1.vue';
import HomeSection2 from '../components/HomeSection2.vue';
import HomeSection3 from '../components/HomeSection3.vue';
import FooterHome from '../components/FooterHome.vue';


  export default {
    name: 'HomeView',
    components: {
      HomeSection1,
      HomeSection2,
      HomeSection3,
      FooterHome
    }
  }
</script>
