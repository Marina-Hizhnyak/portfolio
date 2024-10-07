<template>
    <section class="text-white mt-18" id="skills">
        <div class="absolute right-0 top-[110rem] h-full w-full justify-end">
            <span class="flex opacity-20">
                <span class="w-16 h-32 rounded-l-full flex bg-primary blur-2xl"></span>
                <span class="w-16 h-32 rounded-r-full flex bg-[#f88fc2] blur-2xl mt-14"></span>
            </span>
        </div>
        <div class="md:grid md:grid-cols-2 gap-8 items-center py-8 px-4 xl:gap-16 xl:px-16">
            <!-- Skills Section -->
            <div class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full w-[80%]">
                <h2 class="text-4xl font-bold text-white text-left mb-4">My 
                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">Skills</span>
                </h2>
                <ul class="space-y-4 mt-8 grid grid-cols-1 md:grid-cols-2 gap-4">
                    <li v-for="skill in Skills" :key="skill.id" class="text-lg text-white font-semibold">
                        {{ skill.name }}
                    </li>
                </ul>
            </div>

            <!-- Experience Section -->
<div data-aos="flip-left">
                <h2 class="text-4xl font-bold text-white text-left mb-8 md:text-center md:mt-0 mt-8">My Experiences</h2>
                <div class="space-y-8 py-8" data-aos="fade-left">
                    <div v-for="element in Experinces" :key="element.id"
                    class="flex  items-center rounded-xl p-4 bg-[#111a3e] shadow-lg border border-[#1f1641]"
                    >
                    <div class="w-1/4">
                        <img src="https://img.icons8.com/ios-filled/100/ffffff/lawyer.png" alt="lawyer">
                    </div>
                    <div class="w-3/4 pl-4">
                        <h3 class="text-2xl font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">
                            {{ element.role }}
                        </h3>
                        <p class="text-white">{{ element.company }}</p>
                        <p class="text-white">{{ element.date }}</p>
                    </div>
                </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';
const Skills = ref([
    { id: 1, name: 'HTML5, CSS' },
    { id: 3, name: 'GIT' },
    { id: 4, name: 'GitHub' },
    { id: 5, name: 'WebPack' },
    { id: 6, name: 'Vite' },
    { id: 7, name: 'JavaScript' },
    { id: 8, name: 'PHP' },
    { id: 9, name: 'SQL' },
    { id: 10, name: 'Vue.js' },
    { id: 11, name: 'Laravel' },
    { id: 12, name: 'TailwindCSS' },
    { id: 13, name: 'Bootstrap' },
    { id: 14, name: 'WordPress' },
    { id: 15, name: 'Photoshop' },
]);

const Experinces =ref([
    {
        id:1,
        role:'Accountant',
        company:'Foxtrot - Gostomel',
        date:'September 2018 - April 2022'
    },
    {
        id:2,
        role:'Online Store Manager',
        company:'Independent Company Koulikov',
        date:'January 2017 - August 2018'
    },
])
</script>