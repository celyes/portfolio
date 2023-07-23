<script setup>
import Project from '../components/Project.vue'
import {ref} from "vue";

const projects = ref([
    {
        "title": "Checkr",
        "technology": "Python",
        "link": "https://github.com/celyes/checkr",
        "description": "A Powerful Python library to validate data"
    },
    {
        title: "ESBootcamp",
        technology: "PHP",
        link: "https://getsprint.io",
        description: "Built the website for the first coding bootcamp in Algeria"
    },
    {
        "title": "SimpleMVC",
        "technology": "PHP",
        "link": "https://github.com/celyes/mvc",
        "description": "The simplest and most basic MVC framework"
    },
    {
        "title": "Design Patterns in PHP",
        "technology": "PHP",
        "link": "https://github.com/celyes/design-patterns-php",
        "description": "The most common design patterns written in PHP"
    },
    {
        "title": "Corona Virus tracker",
        "technology": "JavaScript",
        "link": "https://corona-dz.now.sh",
        "description": "The very first Covid-19 tracker for Algeria"
    },
    {
        "title": "i18n",
        "technology": "JavaScript",
        "link": "https://i18n.softvenue.net/",
        "description": "Open source technical terms glossary - English / Arabic"
    },
    {
        "title": "Node Static Server",
        "technology": "Node",
        "link": "https://github.com/celyes/Node-static-server",
        "description": "a really simple Node.js static files server."
    },
    {
        "title": "More works...",
        "technology": "GitHub",
        "link": "https://github.com/celyes?tab=repositories",
        "description": "See other works at GitHub"
    }

])


</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-12 text-center">
                <h3 class="section-title">Previous projects</h3>
                <br/>
            </div>
            <Project v-for="project in projects"
                     :title="project.title"
                     :technology="project.technology"
                     :link="project.link"
                     :description="project.description"
            ></Project>
        </div>
    </div>
</template>