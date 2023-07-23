<script setup>
import ProjectSection from '../components/ProjectsSection.vue'
import TechnologiesSection from "../components/TechnologiesSection.vue";
import PersonalInfoSection from "../components/PersonalInfoSection.vue";
</script>

<template>
    <div class="container py-5">
        <PersonalInfoSection></PersonalInfoSection>
        <br/>
        <hr/>
        <br/>
        <TechnologiesSection></TechnologiesSection>
        <br/>
        <hr/>
        <br/>
        <ProjectSection></ProjectSection>
    </div>
</template>
