<template>
    <div id="about">
        <!-- Custom shape -->
        <div class="custom-shape-divider-top-1666889278" v-if="!isMobile">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" opacity=".25" class="shape-fill"></path>
                <path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" opacity=".5" class="shape-fill"></path>
                <path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" class="shape-fill"></path>
            </svg>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" v-if="isMobile" class="blob-mobile2" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="0.5" d="M0,128L34.3,133.3C68.6,139,137,149,206,170.7C274.3,192,343,224,411,197.3C480,171,549,85,617,90.7C685.7,96,754,192,823,240C891.4,288,960,288,1029,266.7C1097.1,245,1166,203,1234,176C1302.9,149,1371,139,1406,133.3L1440,128L1440,0L1405.7,0C1371.4,0,1303,0,1234,0C1165.7,0,1097,0,1029,0C960,0,891,0,823,0C754.3,0,686,0,617,0C548.6,0,480,0,411,0C342.9,0,274,0,206,0C137.1,0,69,0,34,0L0,0Z"></path></svg>
        <svg xmlns="http://www.w3.org/2000/svg" v-if="isMobile" class="blob-mobile" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="1" d="M0,160L34.3,160C68.6,160,137,160,206,133.3C274.3,107,343,53,411,69.3C480,85,549,171,617,181.3C685.7,192,754,128,823,106.7C891.4,85,960,107,1029,117.3C1097.1,128,1166,128,1234,122.7C1302.9,117,1371,107,1406,101.3L1440,96L1440,0L1405.7,0C1371.4,0,1303,0,1234,0C1165.7,0,1097,0,1029,0C960,0,891,0,823,0C754.3,0,686,0,617,0C548.6,0,480,0,411,0C342.9,0,274,0,206,0C137.1,0,69,0,34,0L0,0Z"></path></svg>
        <!-- Animated background elements -->
        <div class="circle circle1"></div>
        <div class="circle circle2"></div>
        <div class="circle circle3"></div>
        <div class="circle circle4"></div>
        <div class="hat"><img src="@/assets/icons/graduation.png"/></div>
        <div class="pc"><img src="@/assets/icons/monitor.png"/></div>

        <h1 data-aos="zoom-in" data-aos-once="false">About Me</h1>
        <div class="about-container">
            <div class="about1">
                <p data-aos="zoom-in" data-aos-once="false">
                    My very first experience with programming was in high school.<br/> I chose programming as an elective subject because I had always been fascinated by technology. We were taught Javascript during this course and I hated it. The teacher behaved inappropriately and had very mysogynistic attitude, which made his classes very uncomfortable, especially being only one of three girls in the class.
                    I dreaded going to his classes and I barely passed, at this point I thought would never want to do programming again.
                </p>
                <p data-aos="zoom-in" data-aos-once="false" v-if="!isMobile">
                    I started at Kristiania University College in fall of 2020 to pursue a bachelor's degree in frontend and mobile development. There I worked a lot with Javascript, React, Vue and Typescript. I also got to learn app development where I got to build cross platform apps with Ionic, and native apps for iOS (swift) and Android (kotlin). In addition to this I also learned Java, databases, cloud technologies and more. I graduated with a bachelor's degree in June 2023 and got to start at Dr.Dropin as a frontend developer, where I am currently working.                </p>
            </div>
            <div class="about2">
                <p data-aos="zoom-in" data-aos-once="false">
                    After graduating high school in 2019 I started at the Norwegian University of Science and Technology (NTNU), where I started on a bachelor's degree in interactive design. Here I learned about basic design principles, universal design and WCAG, prototyping with Figma and Adobe XD.<br/><br/>
                    During the first semester I also had an introductary coding class where I was taught HTML, CSS and some Javascript, however this time was different. The teacher here made this class so fun and exciting. His classes were the highlight of my week. I got so interested in coding that when I found out that I could become a frontend developer, I dropped out after the first year to pursue an education in tech instead.
                </p>
            </div>
            <div v-if="isMobile">
                <p data-aos="zoom-in" data-aos-once="false">
                    I started at Kristiania University College in fall of 2020 to pursue a bachelor's degree in frontend and mobile development. There I worked a lot with Javascript, React, Vue and Typescript. I also got to learn app development where I got to build cross platform apps with Ionic, and native apps for iOS (swift) and Android (kotlin). In addition to this I also learned Java, databases, cloud technologies and more. I graduated with a bachelor's degree in June 2023 and got to start at Dr.Dropin as a frontend developer, where I am currently working.
                </p>
            </div>
        </div>
        <!-- Custom shape -->
        <div class="custom-shape-divider-bottom-1666895900">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
            </svg>
        </div>
    </div>
</template>

<style scoped>

.blob-mobile {
    position: relative;
    top: -5px;
}
.blob-mobile2 {
    position: absolute;
    top: -5px;
}

h1 {
    margin: 0;
    text-align: center;
    padding-top: 1em;
    font-size: 2.5em;

    @media screen and (min-width: 1024px) {
padding-top: 2.5em;
    
        
    }
}

#about {
    position: relative;
}

.about-container {
    
    
    @media screen and (min-width: 1024px) {
        display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;
    margin-bottom: 5em;
    }
}

.about-container p {
    z-index: 1;
    font-size: clamp(1em, 5vw, 1.2em);
    
    text-align: center;
    padding-bottom: 1em;
    @media screen and (min-width: 1024px) {
        width: 75%;
        padding-bottom: 0;
    }
}

.about1 {
    @media screen and (min-width: 1024px) {
        grid-area: 1 / 1 / 2 / 2;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    flex-direction: column;
    }
    
}

.about2 {
    grid-area: 1 / 2 / 2 / 3; 
    display: flex;
    justify-content: flex-start;
    align-items: center;
}

.about1 p:last-of-type {
    @media screen and (min-width: 1024px) {margin-top: 22.5em;}
    
}

/* Background elements */

.circle {
    position: absolute;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background-color: white;
}

.circle1 {
    top: calc(75% - 75px);
    left: calc(40% - 25px);
    opacity: 0.25;
    animation: float 13s ease-in-out infinite;
}

.circle2 {
    top: calc(25% + 45px);
    left: 13%;
    width: 175px;
    height: 175px;
    opacity: 0.5;
    animation: float2 27s ease-in-out infinite;
    
}

.circle3 {
    top: calc(15%);
    right: 10%;
    opacity: 0.5;
    width: 100px;
    height: 100px;
    animation: float 15s ease-in-out infinite;
}

.circle4 {
    top: calc(78%);
    right: 17%;
    opacity: 0.25;
    width: 200px;
    height: 200px;
    animation: float2 20s ease-in-out infinite;
}

.hat img {
    position: absolute;
    top: calc(30% - 50px);
    right: calc(50% - 450px);
    width: 150px;
    height: 150px;
    animation: float2 20s ease-in-out infinite;
}

.pc img {
    position: absolute;
    top: calc(50%);
    left: calc(50% - 450px);
    width: 150px;
    height: 150px;
    animation: float 26s ease-in-out infinite;
}

/* Floating animations */
@keyframes float {
	0% {

		transform: translatey(0px);
	}
	50% {

		transform: translatey(-20px);
	}
	100% {

		transform: translatey(0px);
	}
}

@keyframes float2 {
	0% {

		transform: translatey(0px);
	}
	50% {

		transform: translatey(20px);
	}
	100% {

		transform: translatey(0px);
	}
}

/* Custom shape */
.custom-shape-divider-top-1666889278 {
    position: relative;
    top: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
}

.custom-shape-divider-top-1666889278 svg {
    position: relative;
    display: block;
    width: calc(121% + 1.3px);
    height: 171px;
    transform: rotateY(180deg);
}

.custom-shape-divider-top-1666889278 .shape-fill {
    fill: #FFFFFF;
}

.custom-shape-divider-bottom-1666895900 {
    position: relative;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1666895900 svg {
    position: relative;
    display: block;
    width: calc(300% + 1.3px);
    height: 154px;
}

.custom-shape-divider-bottom-1666895900 .shape-fill {
    fill: #FFFFFF80;
}
</style>

<script>
export default {
    name: 'AboutSection',
    data() {
        return {
            isMobile: isMobile
        }
    },
}

const isMobile = window.innerWidth <= 1024;
</script>