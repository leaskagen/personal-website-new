<template>
    <div class="technologies-container">
        <div class="tech" v-for="(tech, i) in technologies" :key="i"
                    :image="tech.image"
                    :name="tech.name"
                    data-aos="zoom-in" data-aos-once="false">
            <p><strong>{{tech.name}}</strong></p>
            <img :src="tech.image" alt="tech image" class="tech-image">
        </div>
    </div>
</template>

<script>

export default {
    name: "TechnologiesDiv",
    data: () => ({
        technologies: [
            {
            name: 'HTML',
            image: require('@/assets/technologies/html.png'),
            },
            {
            name: 'CSS',
            image: require('@/assets/technologies/css.png'),
            },
            {
            name: 'Sass',
            image: require('@/assets/technologies/sass.png'),
            },
            {
            name: 'Tailwind',
                image: require('@/assets/technologies/tailwind.png'),
            },
            {
            name: 'Bootstrap',
            image: require('@/assets/technologies/bootstrap.png'),
            },
            {
            name: 'JavaScript',
            image: require('@/assets/technologies/javascript.png'),
            },
            {
            name: 'TypeScript',
            image: require('@/assets/technologies/typescript.png'),
            },
            {
            name: 'Vue.js',
            image: require('@/assets/technologies/vue.png'),
            },
            {
            name: 'React',
            image: require('@/assets/technologies/react.png'),
            },
            {
            name: 'Next.js',
            image: require('@/assets/technologies/next.png'),
            },
            {
            name: 'Swift',
            image: require('@/assets/technologies/swift.png'),
            },
            {
            name: 'Java',
            image: require('@/assets/technologies/java.png'),
            },
            {
            name: 'Kotlin',
            image: require('@/assets/technologies/kotlin.png'),
            },
            {
            name: 'React Native',
            image: require('@/assets/technologies/react.png'),
            },
            {
            name: 'Ionic',
            image: require('@/assets/technologies/ionic.png'),
            },
            {
            name: 'MongoDB',
            image: require('@/assets/technologies/mongodb.png'),
            },
            {
            name: 'Figma',
            image: require('@/assets/technologies/figma.png'),
            },
            {
            name: 'Photoshop',
            image: require('@/assets/technologies/photoshop.png'),
            }
        ],
        isMobile: isMobile
    }),
}

const isMobile = window.innerWidth <= 1024;
</script>

<style scoped>
.technologies-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    row-gap: clamp(1em, 5vw, 2em); 
}

.tech {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    max-width: 100px;
    flex: 1 1 18%;
    @media screen and (max-width: 1024px) {
        flex: 0 0 30%;
    
        
    }
}

.tech p {
    font-size: 1em;
}

.tech-image {
    object-fit: contain;
    height: clamp(3em, 5vw, 3.5em);
    width: auto;
    margin: 0;
}

</style>