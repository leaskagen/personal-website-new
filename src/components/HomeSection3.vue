<template>
    <div id="about">
        <div class="custom-shape-divider-top-1666889278">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M0,0V46.29c47.79,22.2,103.59,32.17,158,28,70.36-5.37,136.33-33.31,206.8-37.5C438.64,32.43,512.34,53.67,583,72.05c69.27,18,138.3,24.88,209.4,13.08,36.15-6,69.85-17.84,104.45-29.34C989.49,25,1113-14.29,1200,52.47V0Z" opacity=".25" class="shape-fill"></path>
                <path d="M0,0V15.81C13,36.92,27.64,56.86,47.69,72.05,99.41,111.27,165,111,224.58,91.58c31.15-10.15,60.09-26.07,89.67-39.8,40.92-19,84.73-46,130.83-49.67,36.26-2.85,70.9,9.42,98.6,31.56,31.77,25.39,62.32,62,103.63,73,40.44,10.79,81.35-6.69,119.13-24.28s75.16-39,116.92-43.05c59.73-5.85,113.28,22.88,168.9,38.84,30.2,8.66,59,6.17,87.09-7.5,22.43-10.89,48-26.93,60.65-49.24V0Z" opacity=".5" class="shape-fill"></path>
                <path d="M0,0V5.63C149.93,59,314.09,71.32,475.83,42.57c43-7.64,84.23-20.12,127.61-26.46,59-8.63,112.48,12.24,165.56,35.4C827.93,77.22,886,95.24,951.2,90c86.53-7,172.46-45.71,248.8-84.81V0Z" class="shape-fill"></path>
            </svg>
        </div>
        <div class="circle circle1"></div>
        <div class="circle circle2"></div>
        <div class="circle circle3"></div>
        <div class="circle circle4"></div>
        <div class="hat"><img src="@/assets/icons/graduation.png"/></div>
        <div class="pc"><img src="@/assets/icons/monitor.png"/></div>
        <h1 data-aos="zoom-in" data-aos-once="false">
            About Me
        </h1>
        <div class="about-container">
            <div class="about1">
                <p data-aos="zoom-in" data-aos-once="false">
                    My very first experience with programming was in high school.<br/> I chose programming as an elective subject because I had always been fascinated by technology. We were taught Javascript during this course and I hated it. The teacher behaved inappropriately and had very mysogynistic attitude, which made his classes very uncomfortable, especially being only one of three girls in the class.
I dreaded going to his classes and I barely passed, at this point I thought would never want to do programming again.
                </p>
                <p data-aos="zoom-in" data-aos-once="false">
                    I started at Kristiania University College in fall of 2020 to pursue a bachelor's degree in frontend and mobile development, and I am still excited about this field. Here I have worked a lot with HTML, CSS and Javascript, and frameworks for these technologies. I have also gotten to learn about new technologies such as React, Java, databases, Kotlin and Android development.<br/> This current semester I am learning about Vue.js, Ionic, iOS development and Swift, Google Cloud and more. I will graduate in spring 2023 and I am looking forward to finally start my career.
                </p>
            </div>
            <div class="about2">
                <p data-aos="zoom-in" data-aos-once="false">After graduating high school in 2019 I started at the Norwegian University of Science and Technology (NTNU), where I started on a bachelor's degree in interactive design. Here I learned about basic design principles, universal design and WCAG, prototyping with Figma and Adobe XD.<br/><br/>

During the first semester I also had an introductary coding class where I was taught HTML, CSS and some Javascript, however this time was different. The teacher here made this class so fun and exciting. His classes were the highlight of my week. I got so interested in coding that when I found out that I could become a frontend developer, I dropped out after the first year to pursue an education in tech instead.

</p>

            </div>

        </div>
        <div class="custom-shape-divider-bottom-1666895900">
            <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z" class="shape-fill"></path>
            </svg>
        </div>
    </div>
</template>

<style scoped>

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

h1 {
        margin: 0;
        text-align: center;
        padding-top: 2.5em;
        font-size: 2.5em;
    }

.about-container {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 0px;
    grid-row-gap: 0px;

    margin-bottom: 5em;
}

.about-container p {
    
    z-index: 1;
    font-size: 1.2em;
    width: 75%;
    text-align: center;
}

.about1 {
    grid-area: 1 / 1 / 2 / 2;
    display: flex;
    justify-content: center;
    align-items: flex-end;
    flex-direction: column;
}

.about2 {
    grid-area: 1 / 2 / 2 / 3; 
    display: flex;
    justify-content: flex-start;
    align-items: center;
}

.about1 p:last-of-type {
    margin-top: 22.5em;
}

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

.circle {
    position: absolute;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background-color: white;
    /*animation: circle 10s ease-in-out infinite;*/
}

.circle1 {
    top: 290%;
    left: 39%;
    /*animation-delay: 0s;*/
    opacity: 0.25;
    animation: float 13s ease-in-out infinite;
}

.circle2 {
    top: 228%;
    left: 13%;
    width: 175px;
    height: 175px;
    /*animation-delay: 0s;*/
    opacity: 0.5;
    animation: float2 27s ease-in-out infinite;
    
}

.circle3 {
    top: 220%;
    right: 10%;
    opacity: 0.5;
    width: 100px;
    height: 100px;
    /*animation-delay: 4s;*/
    animation: float 15s ease-in-out infinite;
}

.circle4 {
    top: 302%;
    right: 17%;
    opacity: 0.25;
    width: 200px;
    height: 200px;
    /*animation-delay: 4s;*/
    animation: float2 20s ease-in-out infinite;
}

.hat img {
    position: absolute;
    top: 233%;
    right: 27%;
    width: 150px;
    height: 150px;
    animation: float2 20s ease-in-out infinite;
}

.pc img {
    position: absolute;
    top: 269.5%;
    left: 27%;
    width: 150px;
    height: 150px;
    animation: float 26s ease-in-out infinite;
}
</style>

<script>
export default {
    name: 'HomeSection3'
}
</script>