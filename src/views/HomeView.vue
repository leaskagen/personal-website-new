<template>
  <main>
    <HeroSection/>
    <HomeSection2/>
    <AboutSection/>
    <FooterHome/>
  </main>
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
import HeroSection from '../components/HeroSection.vue';
import HomeSection2 from '../components/HomeSection2.vue';
import AboutSection from '../components/AboutSection.vue';
import FooterHome from '../components/FooterHome.vue';

  export default {
    name: 'HomeView',
    components: {
      HeroSection,
      HomeSection2,
      AboutSection,
      FooterHome
    }
  }
</script>
