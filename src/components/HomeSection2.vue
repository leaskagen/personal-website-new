<template>
    <div class="section section2" data-anchor="projects" id="projects">
        <h1>Projects</h1>
        <div class="projects-container">
            <div class="project">
                <img src="../assets/meg.jpg" alt="Project 1">
            </div>
            <div class="project">
                <img src="../assets/meg.jpg" alt="Project 1">
            </div>
            <div class="project">
                <img src="../assets/meg.jpg" alt="Project 1">
            </div>
            <div class="project">
                <img src="../assets/meg.jpg" alt="Project 1">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'HomeSection2'

}
</script>

<style scoped>
    .section2 {
        background-color: white;

    }

    h1 {
        margin: 0;
        text-align: center;
        padding-top: 2.5em;
        font-size: 2.5em;
    }

    .projects-container {
        display: flex;
        overflow-x: scroll;
        padding: 24px;
        width: 300px;
        scroll-snap-type: x mandatory;
        scroll-padding: 24px;
        border-radius: 8px;
        gap: 12px;
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

</style>