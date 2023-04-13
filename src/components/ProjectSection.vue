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
                <h2  data-aos="zoom-in" data-aos-once="false">These are some of my best projects</h2>
                <vueper-slides class="no-shadow project-slides" arrows-outside bullets-outside transition-speed="400" fixed-height="60vh" autoplay :touchable="false">
                    <vueper-slide
                        v-for="(slide, i) in slides"
                        :key="i"
                        :image="slide.image"
                        :title="slide.title"
                        :description="slide.description"
                        :techs="slide.techs"
                        :website="slide.website"
                        :github="slide.github"
                        :style="'background: white;'">
                        <template #content>
                            <div class="slide-content">
                                <img :src="slide.image" alt="slide image" class="slide-image"  data-aos="zoom-in" data-aos-once="false">
                                <h3 data-aos="zoom-in" data-aos-once="false">{{ slide.title }}
                                    <a v-if="slide.website != null" :href="slide.website" target="_blank" rel="noopener noreferrer" data-aos="zoom-in" data-aos-once="false"><img src="@/assets/icons/external-link.png" class="link-icon"/></a>
                                    <a v-if="slide.github != null" :href="slide.github" target="_blank" rel="noopener noreferrer" data-aos="zoom-in" data-aos-once="false"><img src="@/assets/icons/github.png" class="link-icon"/></a>
                                </h3>
                                <p data-aos="zoom-in" data-aos-once="false">{{ slide.description }}</p>
                                <p data-aos="zoom-in" data-aos-once="false"><strong>Technologies used: </strong>{{ slide.techs }}</p>
                            </div>
                        </template>
                    </vueper-slide>
                </vueper-slides>
            </div>
        </div>            
    </div>
</template>
<style scoped>

.section2 {
    background-color: white;
    padding-bottom: 5em;
}

h1 {
    margin: 0;
    text-align: center;
    padding-top: 2em;
    padding-bottom: 2em;
    font-size: 2.5em;
    }

h2 {
    text-align: center;
}

h3 {
    margin-bottom: 0;
    font-size: 1.5em;
}

.projects-section {
    display: grid;
    grid-template-columns: 40% 60%;
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}

.projects-right {
    grid-area: 1 / 2 / 2 / 3;
    padding: 0 2em;
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

/* Project slides */
.project-slides {
  width: 85%;
  max-width: 90%;
  margin: auto;
}

.slide-content {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.slide-image {
    width: 80%;
    max-width: 700px;
    height: auto;
    filter: drop-shadow(0px 4px 6px rgba(0, 0, 0, 0.3));
}

.slide-content p {
    font-size: 1em;
    text-align: center;
}

.link-icon {
    width: 1em;
    height: 1em;
    margin-left: 0.25em;
}

</style>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'

import TechnologiesDiv from './Technologies.vue';

export default {
    data: () => ({
        slides: [
            {
            title: 'Gyldne Pizza Portalen',
            image: require('@/assets/screenshots/screenshot-1.png'),
            description: 'I made this project with a few other students for an exam we had in the second semester (spring 2021). This website was made for the employees in charge of a fictional resturant chain. Here you can see statistics for different restaurants and menu items, add or remove employees, edit menu items, and a few other things you would want to do as an employee or manager.',
            techs: 'HTML, CSS, Bulma, Javascript, Google Charts',
            website: 'https://runejac.github.io/WebprosjektSolution/index.html',
            github: 'https://github.com/runejac/webprosjekt'
            },
            {
            title: 'Pizzeria Bella',
            image: require('@/assets/screenshots/pizzeria_bella.png'),
            description: 'This is another group project I did during the third semester (fall 2021). The project was made for a fictional pizza resturant, where customers can order pizza by adding or removing items from their shopping cart. This was also the very first project we made with React, and it is optimalized for desktop, tablet and phone screen sizes.',
            techs: 'HTML, CSS, React',
            website: null,
            github: 'https://github.com/leaskagen/eksamen-grensesnittdesign'
            },
            {
            title: 'Meliora Impact',
            image: require('@/assets/screenshots/screenshot-2.png'),
            description: 'This is one of the most complex projects that I have been a part of, it was made for my most recent exam and I made it with my group. The project was made for Meliora Impact which is a Norwegian non profit. They wanted a platform where small-medium sized businesses can subscribe to charities, meaning that they donate to them regularly.',
            techs: 'React, CSS, Google OpenID, MongoDB, Express.js, Heroku',
            website: "https://pro201-smidig.herokuapp.com/",
            github: "https://github.com/a-baade/pro201-smidig"
            },
            {
            title: 'Old Personal Website',
            image: require('@/assets/screenshots/personal.png'),
            description: 'This is my first personal website I built trying out Fullpage.js and Sass. It was a small and fun side project I did in my spare time earlier this year. It is also translated to both English and Norwegian.',
            techs: 'HTML, Sass, Javascript, Fullpage.js',
            website: 'https://leaskagen.github.io/',
            github: 'https://github.com/leaskagen/leaskagen.github.io'
            },
            {
            title: 'Retro Trader App',
            image: require('@/assets/screenshots/retroapp.svg'),
            description: 'This is a crossplattform app I made with Ionic framework with Vue.js and Typescript, also with Directus as database and backend. It was made for an exam in the fifth semester (fall 2022) and is a marketplace for retro games. You can create an account, publish games for sale, buy games, chat with other users, and more.',
            techs: 'Ionic, Vue.js, Typescript, Directus, GraphQL, iOS/Xcode, Capacitor, Google Maps API',
            website: null,
            github: 'https://github.com/leaskagen/Eksamen-Kryssplattform'
            },
            {
            title: 'Fruity App',
            image: require('@/assets/screenshots/fruity.svg'),
            description: 'This is a native iOS app I made with Swift and Xcode for an exam in the fifth semester (fall 2022). It gets fruits from an API and you can see them in a list or grouped by different categories. You can also save eaten fruits in core data and see a log of different fruits you have eaten in a list that is sorted by date.',
            techs: 'Xcode, Swift, Storyboard, Core Data, API',
            website: null,
            github: 'https://github.com/leaskagen/Eksamen-iOS-Programmering'
            }
            ,
            {
            title: 'Stimulating Split Screen Chrome Extension',
            image: require('@/assets/screenshots/extension2.jpg'),
            description: 'This project is inspired by the overstimulation trends on TikTok, where people add relaxing gameplay or other satisfying videos next to clips of for example Family Guy to keep your attention. I made this Chrome extension where you can watch relaxing videos in a split screen next to whatever you are doing with just one click.',
            techs: 'Javascript, HTML, CSS, Chrome Extension API Manifest Version 3',
            website: 'https://chrome.google.com/webstore/detail/stimulating-split-screen/eiofmldbnffekfojgldjgeebnjeblhgc?hl=en&authuser=0',
            github: 'https://github.com/leaskagen/Stimulating-Split-Screen-Chrome-Extension'
            }
        ]
    }),
        components: {
        VueperSlides, 
        VueperSlide,
        TechnologiesDiv
    },
}

</script>