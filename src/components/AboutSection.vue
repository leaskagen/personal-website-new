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
        <div class="circle circle1">
            <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#FFFFFF" fill-opacity="25%" d="M41.6,-75.1C51,-66.8,53.4,-49.5,61,-35.5C68.7,-21.5,81.5,-10.7,84.5,1.7C87.5,14.2,80.7,28.4,69.4,36.1C58.2,43.9,42.4,45.1,30.1,54.1C17.8,63.1,8.9,80,-2.5,84.4C-14,88.8,-27.9,80.7,-40.2,71.6C-52.5,62.5,-63,52.5,-68.1,40.4C-73.1,28.3,-72.6,14.2,-73.7,-0.6C-74.8,-15.4,-77.5,-30.9,-70.3,-39.2C-63.1,-47.6,-46.1,-48.9,-32.7,-55C-19.3,-61,-9.7,-71.8,3.2,-77.4C16.2,-83,32.3,-83.5,41.6,-75.1Z" transform="translate(100 100)" />
            </svg>
        </div>
        <div class="circle circle2">
            <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#FFFFFF" fill-opacity="50%" d="M37.7,-60.4C50.6,-57.8,64,-51.3,70.7,-40.5C77.4,-29.8,77.4,-14.9,74.3,-1.8C71.1,11.3,64.9,22.6,57.2,31.6C49.6,40.7,40.5,47.5,30.7,51.7C20.9,55.9,10.5,57.4,0.9,55.9C-8.8,54.4,-17.5,49.9,-26.8,45.5C-36.1,41.1,-46,36.7,-54.5,29.1C-63,21.5,-70.1,10.7,-73.1,-1.7C-76.2,-14.2,-75.1,-28.5,-67.3,-37.3C-59.5,-46.1,-45,-49.4,-32.6,-52.4C-20.3,-55.4,-10.2,-58.1,1.1,-60C12.4,-61.9,24.7,-63.1,37.7,-60.4Z" transform="translate(100 100)" />
            </svg>
        </div>
        <div class="circle circle3">
            <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#FFFFFF" fill-opacity="50%" d="M24.1,-47.6C31.5,-37.6,37.9,-31.5,47.9,-24.3C57.9,-17,71.7,-8.5,75.2,2C78.6,12.5,71.9,25.1,64.4,36.8C56.9,48.4,48.7,59.2,37.8,62.3C26.9,65.4,13.5,60.8,0.3,60.4C-12.9,59.9,-25.9,63.5,-38,61.2C-50.1,58.8,-61.5,50.4,-69.2,39.3C-76.8,28.1,-80.8,14,-79.7,0.6C-78.6,-12.7,-72.4,-25.5,-66.6,-39.9C-60.8,-54.3,-55.3,-70.4,-44.3,-78.3C-33.3,-86.3,-16.6,-86.1,-4.1,-78.9C8.4,-71.8,16.8,-57.7,24.1,-47.6Z" transform="translate(100 100)" />
            </svg>
        </div>
        <div class="circle circle4">
            <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
                <path fill="#FFFFFF" fill-opacity="25%" d="M40.3,-67.4C52.4,-62.9,62.4,-52.3,66.8,-40.1C71.3,-27.9,70.2,-13.9,70.4,0.1C70.5,14.1,71.8,28.1,68,41.6C64.2,55,55.4,67.9,43.2,76.9C31.1,86,15.5,91.3,2,87.9C-11.6,84.5,-23.2,72.4,-32.5,61.7C-41.8,50.9,-48.7,41.5,-55.9,31.5C-63.1,21.4,-70.7,10.7,-75.6,-2.8C-80.5,-16.4,-82.8,-32.8,-77.8,-46.7C-72.8,-60.6,-60.5,-71.9,-46.3,-75.3C-32.1,-78.6,-16,-73.9,-1,-72.2C14.1,-70.6,28.3,-72,40.3,-67.4Z" transform="translate(100 100)" />
            </svg>
        </div>
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
    width: 200px;
    height: 200px;
    /*
    border-radius: 50%;
    background-color: white;
    */
}

.circle1 {
    top: calc(75% - 75px);
    left: calc(40% - 25px);
    /*
    opacity: 0.25;
    */
    animation: float 13s ease-in-out infinite;
}

.circle2 {
    top: calc(25% + 5px);
    left: 13%;
    width: 375px;
    height: 375px;
    /*
    opacity: 0.5;
    */
    animation: float2 27s ease-in-out infinite;
    
}

.circle3 {
    top: calc(15%);
    right: 10%;
    /*
    opacity: 0.5;
    */
    width: 200px;
    height: 200px;
    animation: float 15s ease-in-out infinite;
}

.circle4 {
    top: calc(75%);
    right: 17%;
    /*
    opacity: 0.25;
    */
    width: 300px;
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