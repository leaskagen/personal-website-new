<template>
    <footer id="contact">
        <h1>Contact me</h1>
        
            <ul>
                <li>
                    <a href="https://www.linkedin.com/in/lea-sofie-skagen-a29451169">
                        <img src="@/assets/icons/linkedin.png" alt="link to my linkedin"> Lea Sofie Skagen
                    </a>
                </li>
                <li>
                    <a href="https://github.com/leaskagen">
                        <img src="@/assets/icons/github.png" alt="link to my github"> leaskagen
                    </a>
                </li>
                <li>
                    <a href="mailto:lea.skagen@gmail.com">
                        <img src="@/assets/icons/mail.png" alt="send me email"> lea.skagen@gmail.com
                    </a>
                </li>
                <li>
                    <a href="https://leaskagen.github.io/resume.html" target="_blank" rel="noopener noreferrer">
                        <img src="@/assets/icons/resume.png" alt="send me email"> See my resume
                    </a>
                </li>
            </ul>
            <p class="bottom-text">This website was made with Vue.js<br/>Shapes are made with <a href="https://www.shapedivider.app" target="_blank" rel="noopener noreferrer">shapedivider.app</a> and icons are from <a href="https://www.flaticon.com/" target="_blank" rel="noopener noreferrer">flaticon.com</a> and <a href="https://freeicons.io/" target="_blank" rel="noopener noreferrer">freeicons.io</a></p>
        
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
        margin: 1vh 0;
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
    name: 'FooterHome'
}
</script>