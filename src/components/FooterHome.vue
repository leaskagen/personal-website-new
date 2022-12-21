// This is the footer component for the page
<template>
    <footer id="contact">
        <h1 data-aos="zoom-in" data-aos-once="false">Contact me</h1>
        <ul v-for="(link, i) in links" :key="i"
                    :link="link.link"
                    :image="link.image"
                    :text="link.text"
                    :alt="link.alt">
            <li data-aos="zoom-in" data-aos-once="false">
                <a :href="link.link">
                    <img :src="link.image" :alt="link.alt"> {{link.text}}
                </a>
            </li>
        </ul>
        <p class="bottom-text" data-aos="zoom-in" data-aos-once="false">This website was made with Vue.js, link to repository for this project <a href="https://github.com/leaskagen/personal-website-new" target="_blank" rel="noopener noreferrer">here</a>.<br/>Shapes are made with <a href="https://www.shapedivider.app" target="_blank" rel="noopener noreferrer">shapedivider.app</a> and icons are from <a href="https://www.flaticon.com/" target="_blank" rel="noopener noreferrer">flaticon.com</a> and <a href="https://freeicons.io/" target="_blank" rel="noopener noreferrer">freeicons.io</a></p>
    </footer>
</template>

<style>
footer {
    background-color: #FFFFFF80;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-bottom: 5em;
}

h1 {
    margin: 0;
    padding-bottom: 1.5em;
}

ul {
        list-style-type: none;
        width: 350px;
}

li {
    margin:  0;
    font-size: 14px;
    text-align: left;
}

p {
    font-size: 14px;
}

img {
    height: 30px;
    position: relative;
    top: 5px;
    margin-right: 10px;
    fill: #202020;
}

a {
    color: #202020;
    text-decoration: none;
    font-size: 24px;
}

a:hover {
    text-decoration: underline;
}

.bottom-text {
    margin-top: 5em;
    text-align: center;
    font-size: 14px;
}

.bottom-text a {
    font-size: 14px;
    text-decoration: underline;
}
</style>

<script>
export default {
    name: 'FooterHome',
    data: () => ({
        links: [
            {
            link: 'https://www.linkedin.com/in/lea-sofie-skagen-a29451169',
            image: require('@/assets/icons/linkedin.png'),
            text: 'Lea Sofie Skagen',
            alt: 'link to my linkedin'
            },
            {
            link: 'https://github.com/leaskagen',
            image: require('@/assets/icons/github.png'),
            text: 'leaskagen',
            alt: 'link to my github'
            },
            {
            link: 'mailto:lea.skagen@gmail.com',
            image: require('@/assets/icons/mail.png'),
            text: 'lea.skagen@gmail.com',
            alt: 'send me an email'
            },
            {
            link: 'https://leaskagen.github.io/resume.html',
            image: require('@/assets/icons/resume.png'),
            text: 'See my resume',
            alt: 'See my resume'
            }  
        ]
    }),
}
</script>