<template>
    <div class="section section2" data-anchor="projects" id="projects">
        <h1 data-aos="zoom-in" data-aos-once="false">Projects</h1>
        <div class="projects-section">
            <div class="projects-left">
                <h2 data-aos="zoom-in" data-aos-once="false">Technologies</h2>
                <p data-aos="zoom-in" data-aos-once="false">These are the technologies I have worked with before or am currently learning</p>
                <TechnologiesDiv />
            </div>
            <div class="projects-right">
                <h2  data-aos="zoom-in" data-aos-once="false">These are projects I have worked on before</h2>
                <vueper-slides class="no-shadow project-slides" arrows-outside bullets-outside transition-speed="400" fixed-height="60vh" autoplay>
                <vueper-slide
                    v-for="(slide, i) in slides"
                    :key="i"
                    :image="slide.image"
                    :title="slide.title"
                    :description="slide.description"
                    :techs="slide.techs"
                    :style="'background: white;'">
                    <template #content>
                        <div class="slide-content">
                            <img :src="slide.image" alt="slide image" class="slide-image"  data-aos="zoom-in" data-aos-once="false">
                            <h3  data-aos="zoom-in" data-aos-once="false">{{ slide.title }}</h3>
                            <p  data-aos="zoom-in" data-aos-once="false">{{ slide.description }}</p>
                            <p  data-aos="zoom-in" data-aos-once="false"><strong>Technologies used: </strong>{{ slide.techs }}</p>
                        </div>
                    </template>
                </vueper-slide>
                </vueper-slides>
            
        </div>
            </div>
            
        </div>
</template>
<style scoped>

.project-slides {

  width: 85%;
  max-width: 90%;
  margin: auto;
}

.slide-content {
    display: flex;
    flex-direction: column;
    
}

.slide-content p {
    font-size: 1em;
    text-align: center;
}

.slide-image {
    width: 80%;
    max-width: 700px;
    height: auto;
    filter: drop-shadow(0px 4px 6px rgba(0, 0, 0, 0.3));
}
.projects-left {
    grid-area: 1 / 1 / 2 / 2;
    padding: 0 2em;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.projects-left p {
    font-size: 1em;
}

.projects-right {
    grid-area: 1 / 2 / 2 / 3;
    padding: 0 2em;
}

h2 {
    text-align: center;
}

h3 {
    margin-bottom: 0;
}

/*<div class="buttons">
                <button  @click="next">next</button>
                <button  @click="prev">prev</button>
            </div>
            <div class="projectslides">
                <div class="project-slide">
                    <img src="@/assets/screenshots/screenshot-1.png" alt="project screenshot">
                    <div class="project-content">
                        <h3>Gyldne Pizza Portalen</h3>
                        <p>I made this project with a few other students for an exam we had in the second semester (spring 2021). This website was made for the employees in charge of a fictional resturant chain. Here you can see statistics for different restaurants and menu items, add or remove employees, edit menu items, and a few other things you would want to do as an employee or manager.</p>
                        <p><strong>Technologies used:</strong> HTML, CSS, Bulma, Javascript, Google Charts</p>
                    </div>
                </div>
                <div class="project-slide">
                    <img src="@/assets/screenshots/screenshot-1.png" alt="project screenshot">
                    <div class="project-content">
                        <h3>Gyldne Pizza Portalen</h3>
                        <p>I made this project with a few other students for an exam we had in the second semester (spring 2021). This website was made for the employees in charge of a fictional resturant chain. Here you can see statistics for different restaurants and menu items, add or remove employees, edit menu items, and a few other things you would want to do as an employee or manager.</p>
                        <p><strong>Technologies used:</strong> HTML, CSS, Bulma, Javascript, Google Charts</p>
                    </div>
                </div>
                <div class="project-slide">
                    <img src="@/assets/screenshots/screenshot-1.png" alt="project screenshot">
                    <div class="project-content">
                        <h3>Gyldne Pizza Portalen</h3>
                        <p>I made this project with a few other students for an exam we had in the second semester (spring 2021). This website was made for the employees in charge of a fictional resturant chain. Here you can see statistics for different restaurants and menu items, add or remove employees, edit menu items, and a few other things you would want to do as an employee or manager.</p>
                        <p><strong>Technologies used:</strong> HTML, CSS, Bulma, Javascript, Google Charts</p>
                    </div>
                </div>*/
    .section2 {
        background-color: white;
        padding-bottom: 5em;
        /*height: 120vh;*/

    }

    h1 {
        margin: 0;
        text-align: center;
        padding-top: 2em;
        padding-bottom: 2em;
        font-size: 2.5em;
    }

    .projectslides {
    width: 90%;
    height: 100%;
    margin: auto;
    white-space: nowrap;
    display: flex;

    
}


.projects-section {
    display: grid;
    grid-template-columns: 40% 60%;
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}

.slide-content {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    
}
.project-content {
    padding-top: 1em;
    text-align: center;
}
h3 {
    font-size: 1.5em;
}
.project-content p {
    z-index: 10;
    font-size: 1em;
    
}
.project-slide {
    height: 72vh;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 60%;
    max-width: 60%;
    margin: auto;
    white-space: normal;
}

.project-slide img {
    height: 100%;
    width: 100%;
    filter: drop-shadow(5px 0px 9px #CECECE);
}

    .splide__slide {
        width: 100vw;
        /*
        height: 70vhpx;
        width: 90vw;
        */
    }

    .splide__slide img {
        height: 100%;
        width: 90vw;
        object-fit: cover;
    }
    /*
<div class="project-aside">
                <p>Here are some of the projects I have worked on in the past.</p>

                <h2>These are the technologies I have worked with</h2>
            </div>
            <div class="projects-container">
                <splide :options="options">
                    <splide-slide class="splide__slide">
                    <img src="@/assets/screenshots/screenshot-1.png">
                    </splide-slide>
                    <splide-slide class="splide__slide">
                    <img src="@/assets/meg.jpg">
                    </splide-slide>
                    <splide-slide class="splide__slide">
                    <img src="@/assets/meg.jpg">
                    </splide-slide>
                </splide>
            </div>
    */
    /*
    .projects-section {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: 1fr;
        grid-column-gap: 0px;
        grid-row-gap: 0px;
    }

    .vueperslides__arrow {color: yellow}
*/
    /*
    .project-aside {
        grid-area: 1 / 1 / 2 / 2;
    }
    img {
        height: 500px;
        width: 800px;
        object-fit: cover;
    }
    .splide__slide {
        height: 500px;
        width: 800px;
    }

    .projects-container {
        grid-area: 1 / 2 / 2 / 3;
        width: 80%;
    }
*/
    /*
    .projects-container {
        display: flex;
        overflow-x: scroll;
        padding: 24px;
        width: 300px;
        scroll-snap-type: x mandatory;
        scroll-padding: 24px;
        border-radius: 8px;
        gap: 12px;
        grid-area: 1 / 2 / 2 / 3;
    }

    .projects-container .project {
        flex: 0 0 100%;
        padding: 24px;
        border-radius: 8px;
        scroll-snap-align: start;
    }

    .projects-container .project img {
        width: 250px;
        height: 100%;
        object-fit: cover;
        border-radius: 8px;
    }
*/
</style>

<script>
// In your Vue.js component.
/*
import '@splidejs/splide/dist/css/themes/splide-default.min.css';
import { Splide, SplideSlide } from '@splidejs/vue-splide';
*/

import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'

import TechnologiesDiv from './Technologies.vue';

//import Flicking from "@egjs/vue3-flicking";

export default {

    data: () => ({
slides: [
    {
      title: 'Gyldne Pizza Portalen',
      image: require('@/assets/screenshots/screenshot-1.png'),
      description: 'I made this project with a few other students for an exam we had in the second semester (spring 2021). This website was made for the employees in charge of a fictional resturant chain. Here you can see statistics for different restaurants and menu items, add or remove employees, edit menu items, and a few other things you would want to do as an employee or manager.',
      techs: 'HTML, CSS, Bulma, Javascript, Google Charts'
    },
    {
      title: 'Pizzeria Bella',
      image: require('@/assets/screenshots/pizzeria_bella.png'),
      description: 'This is another group project I did during the third semester (fall 2021). The project was made for a fictional pizza resturant, where customers can order pizza by adding or removing items from their shopping cart. This was also the very first project we made with React, and it is optimalized for desktop, tablet and phone screen sizes.',
      techs: 'HTML, CSS, React'
    },
    {
      title: 'Meliora Impact',
      image: require('@/assets/screenshots/screenshot-2.png'),
      description: 'This is the most complex project I have been a part of yet, it was made for my most recent exam and I made it with my group. The project was made for Meliora Impact which is a Norwegian non profit. They wanted a platform where small-medium sized businesses can subscribe to charities, meaning that they donate to them regularly.',
      techs: 'React, CSS, Google OpenID, MongoDB, Express.js, Heroku'
    }
  ]
}),
    components: {
    VueperSlides, 
    VueperSlide,
    TechnologiesDiv
    },
    //Splide,
    //SplideSlide
    }




  

    /*data () {
    return {
      // ...
      innerStyles: {},
      step: ''
    }
  },

  mounted () {
    this.setStep()
  },

  methods: {
    setStep () {
      const innerWidth = this.$refs.projectslides.scrollWidth // ❶
      const totalCards = 3
      this.step = `${innerWidth / totalCards}px` // ❷
    },

    next () {
      this.moveLeft() // ❸
    },

    moveLeft () {
      this.innerStyles = {
        transform: `translateX(-${this.step})`
      }
    }
  }
  ,components: {
    Flicking: Flicking
  }
}*/
/*
    data: () => ({
slides: [
    { content: '<div><img src=</div>'}
    //{ image: require('@/assets/screenshots/screenshot-1.png'), title: 'Gyldne Pizza Portalen' },
    //{ title: 'Time', content: 'Time in 5 hours: ' }
  ]
}),
*/
    /*
    data() {
      return {
        options: {
            rewind  : true,
            gap     : '1rem',
            autoplay: true,
            height  : '45rem',


        },
      };
    },*/
    //name:'HomeSection2',
    
  



</script>