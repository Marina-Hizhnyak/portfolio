<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar/>
    <HeroSection/>
    <ServicesSection/>
    <AboutSection/>
    <ExperiencesSkills/>
     <Projects/>
    <Contact/>
    <Footer/>
  </div>
</template>

<script setup>
import { defineAsyncComponent } from 'vue';
// import Components 
const NavBar = defineAsyncComponent(() => import('@/components/NavBar.vue'));
const HeroSection = defineAsyncComponent(() => import('@/components/HeroSection.vue'));
// const ServicesSection = defineAsyncComponent(() => import('@/components/ServicesSection.vue'));
const AboutSection = defineAsyncComponent(() => import('@/components/AboutSection.vue'));
const ExperiencesSkills = defineAsyncComponent(() => import('@/components/ExperiencesSkills.vue'));
const Projects = defineAsyncComponent(()=>import('@/components/Projects.vue'));
const Contact = defineAsyncComponent(()=>import('@/components/Contact.vue'));
const Footer = defineAsyncComponent(()=>import('@/components/Footer.vue'));
</script>

