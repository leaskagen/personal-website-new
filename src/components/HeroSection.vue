<template>
    <div class="section section1" data-anchor="welcome" id="welcome">
        <div class="circle circle1"></div>
        <div class="circle circle2"></div>
        <div class="circle circle3"></div>
        <div class="container">
            <div class="div1">
                <h1 data-aos="zoom-in" data-aos-once="false" data-aos-duration="1500">Lea Skagen</h1>
                <h2 data-aos="zoom-in" data-aos-once="false" data-aos-duration="1500">Frontend & App Developer</h2>
                <p data-aos="zoom-in" data-aos-once="false" data-aos-duration="1500">My name is Lea, and I am currently {{ age }} years old and live in Oslo, Norway. I graduated with a bachelor's degree in frontend and mobile development in June 2023, and I am currently working as a frontend developer at Dr.Dropin</p>
            </div>
            <div class="div2" v-if="!isMobile">
                <img src="@/assets/meg.jpg" data-aos="zoom-in" data-aos-once="false" data-aos-duration="2000"/>
            </div>
        </div>
        <!-- Custom shape -->
        <div class="custom-shape-divider-bottom-1666873237" v-if="!isMobile">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" opacity=".25" class="shape-fill"></path>
                <path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" opacity=".5" class="shape-fill"></path>
                <path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" class="shape-fill"></path>
            </svg>
        </div>
        <svg v-if="isMobile" class="blob-mobile" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="1" d="M0,64L60,80C120,96,240,128,360,128C480,128,600,96,720,106.7C840,117,960,171,1080,165.3C1200,160,1320,96,1380,64L1440,32L1440,320L1380,320C1320,320,1200,320,1080,320C960,320,840,320,720,320C600,320,480,320,360,320C240,320,120,320,60,320L0,320Z"></path></svg>
        <svg v-if="isMobile" class="blob-mobile2" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="0.54" d="M0,256L48,234.7C96,213,192,171,288,154.7C384,139,480,149,576,170.7C672,192,768,224,864,224C960,224,1056,192,1152,170.7C1248,149,1344,139,1392,133.3L1440,128L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>
    </div>
</template>

<script>
export default {
    name: 'HeroSection',
    data() {
        return {
            isMobile: isMobile,
            age: age
        }
    }
}

function calculate_age(dob) { 
    var diff_ms = Date.now() - dob.getTime();
    var age_dt = new Date(diff_ms); 
  
    return Math.abs(age_dt.getUTCFullYear() - 1970);
}

const isMobile = window.innerWidth <= 1024;
const age = calculate_age(new Date(2000, 7, 28));
</script>

<style scoped>

.section1 {
    @media screen and (max-width: 1024px) {
        width: 100vw;
        height: 100vh;
        display: flex;
        flex-direction: column;
        padding-bottom: 0;
        justify-content: space-between;
    }
}

.blob-mobile {
    position: absolute;
    bottom: -10px;
}
.blob-mobile2 {
    position: absolute;
    bottom: 1px;
}

.container {
    @media screen and (min-width: 1024px) {
       display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 75vh;
    grid-column-gap: 0px;
    grid-row-gap: 0px; 
    }
    
}

.div1 { 
    padding: 2.5em;
    padding-top: 5em;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    @media screen and (min-width: 1024px) {
        padding-left: 13em;
    
    grid-area: 1 / 1 / 2 / 2; 
    }
    
}

.div2 { 
    grid-area: 1 / 2 / 2 / 3; 
    display: flex;
    justify-content: center;
    align-items: center;
    padding-right: 6em;
    padding-top: 5em;
}

.div2 img {
    width: 60%;
    max-width: 350px;
}

h1 {
    font-size: 3em;
}

p {
    text-align: center;
    font-size: 1.2em;
    z-index: 1;
}

img {
    border-radius: 50%;
    width: 325px;
    height: auto;
    z-index: 1;
    animation: float2 30s ease-in-out infinite;
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
    top: 10%;
    left: 36%;
    opacity: 0.25;
    animation: float 13s ease-in-out infinite;
}

.circle2 {
    top: 36%;
    left: 8%;
    width: 175px;
    height: 175px;
    opacity: 0.5;
    animation: float2 27s ease-in-out infinite;
    
}

.circle3 {
    bottom: 26%;
    right: 5%;
    opacity: 0.25;
    width: 200px;
    height: 200px;
    animation: float 12s ease-in-out infinite;
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
.custom-shape-divider-bottom-1666873237 {
    position: relative;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
    transform: rotate(180deg);
}

.custom-shape-divider-bottom-1666873237 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 191px;
}

.custom-shape-divider-bottom-1666873237 .shape-fill {
    fill: #FFFFFF;
}
</style>