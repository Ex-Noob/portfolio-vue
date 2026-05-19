<template>
    <section class="relative py-20 overflow-hidden" id="projects">
        <div class="relative z-10 max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <!-- Section Header -->
            <div class="text-center mb-16" data-aos="fade-up">
                <h2 class="text-4xl md:text-5xl font-bold text-white mb-4">
                    My <span class="text-transparent bg-clip-text bg-linear-to-r from-blue-400 to-cyan-400">
                        Projects
                    </span>
                </h2>
                <p class="text-blue-200 text-lg max-w-2xl mx-auto">
                    A collection of my recent work and creative solutions
                </p>
            </div>

            <!-- Projects Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div v-for="(project, index) in projects" :key="project.id"
                    class="group relative bg-linear-to-br from-gray-800/50 to-blue-900/30 rounded-3xl overflow-hidden border backdrop-blur-sm hover:border-blue-400/40 transition-all duration-500 hover:transform hover:-translate-y-2"
                    :class="project.bordColor" data-aos="fade-up" :data-aos-delay="(index + 1) * 100">
                    <!-- Project Image -->
                    <div class="relative overflow-hidden">
                        <img :src="project.image" :alt="project.title"
                            class="w-full h-48 object-cover group-hover:scale-110 transition-transform duration-500">
                        <div class="absolute inset-0 bg-linear-to-t from-gray-900 via-transparent to-transparent">
                        </div>
                        <div class="absolute top-4 right-4">
                            <span class="px-3 py-1 text-white text-xs rounded-full font-semibold"
                                :class="project.badgColor">
                                {{ project.category }}
                            </span>
                        </div>
                    </div>
                    <!-- Project Content -->
                    <div class="p-6">
                        <h3
                            class="text-xl font-bold text-white mb-2 group-hover:text-blue-400 transition-colors duration-300">
                            {{ project.title }}
                        </h3>
                        <p class="text-blue-100 text-sm leading-relaxed mb-4">
                            {{ project.desc }}
                        </p>
                        <!-- Technologies -->
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span v-for="tech in project.technolg" :key="tech.name"
                                class="px-2 py-1 border rounded text-xs"
                                :class="tech.class">
                                {{ tech.name }}
                            </span>
                        </div>
                        <!-- Project Links -->
                        <div class="flex gap-3">
                            <a v-for="link in project.links" :key="link.name" :href="link.url" :class="link.class"
                                target="_blank" rel="noopener noreferrer"
                                class="flex items-center gap-2 transition-colors duration-300 text-sm font-medium">
                                <component :is="link.icon" class="w-4 h-4" />
                                {{ link.name }}
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <!-- CTA Section -->
            <div class="text-center mt-16" data-aos="fade-up">
                <div class="inline-flex flex-col sm:flex-row gap-4 items-center">
                    <button
                        class="px-8 py-4 rounded-xl bg-linear-to-r from-blue-500 to-cyan-500 text-white font-semibold hover:shadow-lg hover:shadow-blue-500/25 transition-all duration-300 hover:scale-105 flex items-center">
                        View All Projects
                        <ArrowRightIcon class="w-5 h-5 ml-2" />
                    </button>
                    <button
                        class="px-8 py-4 rounded-xl border-2 border-blue-400 text-blue-400 font-semibold hover:bg-blue-400/10 transition-all duration-300 flex items-center">
                        <ChatBubbleLeftRightIcon class="w-5 h-5 mr-2" />
                        Discuss Project
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import {
    ArrowRightIcon,
    ChatBubbleLeftRightIcon,
    ClockIcon,
    CodeBracketIcon,
    EyeIcon
} from '@heroicons/vue/16/solid';
import { ref } from 'vue';

const projects = ref([
    
    {
        id: 1,
        title: "E-Commerce Website",
        desc: "A fully functional e-commerce website built with React JS, Tailwind CSS and Context API. Features include product listings, cart management, and a clean responsive UI — all handled with React state and Context API, no backend required.",
        image: '/project1.png', 
        category: 'React',
        bordColor: 'border-blue-500/20',
        badgColor: 'bg-blue-500',
        technolg: [
            { name: "React JS",     class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "Tailwind CSS", class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
            { name: "Context API",  class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://e-commerce-46.netlify.app/",
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/e-commerce",
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

    {
        id: 2,
        title: "Portfolio Website",
        desc: "A personal portfolio website built with JS and CSS. Fully responsive with smooth animations, a skills section, projects showcase, and contact form. Currently being customized and improved.",
        image: '/project2.png', 
        category: 'JS',
        bordColor: 'border-cyan-500/20',
        badgColor: 'bg-cyan-500',
        technolg: [
            { name: "HTML",       class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
            { name: "CSS", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "JavaScript", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://your-portfolio-live-url.netlify.app", 
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/Portfolio-Website", 
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

    
    {
        id: 3,
        title: "Personal Portfolio Page",
        desc: "An earlier portfolio project built with pure HTML, CSS and a touch of JavaScript. Clean layout with hero, about, and projects sections — no frameworks, just solid fundamentals.",
        image: '/project3.png', 
        category: 'HTML/CSS',
        bordColor: 'border-blue-500/20',
        badgColor: 'bg-blue-600',
        technolg: [
            { name: "HTML",       class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "CSS",        class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
            { name: "JavaScript", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://your-old-portfolio.netlify.app", 
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/portfolio-Page", 
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

    {
        id: 4,
        title: "Business Landing Page",
        desc: "A professional business landing page with a hero section, services, and CTA. Built with HTML and CSS — clean layout focused on visual hierarchy and responsiveness.",
        image: '/project4.png', 
        category: 'HTML/CSS',
        bordColor: 'border-cyan-500/20',
        badgColor: 'bg-cyan-600',
        technolg: [
            { name: "HTML", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "CSS",  class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://your-business-page.netlify.app", 
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/businessLandingPage",
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

    
    {
        id: 5,
        title: "Tribute — Dr. Abdul Qadeer Khan",
        desc: "A tribute page honouring Dr. Abdul Qadeer Khan, the father of Pakistan's nuclear programme. Built with HTML and CSS, focused on clean typography, layout, and respectful presentation.",
        image: '/project5.png', 
        category: 'HTML/CSS',
        bordColor: 'border-blue-500/20',
        badgColor: 'bg-blue-500',
        technolg: [
            { name: "HTML", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "CSS",  class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://your-tribute-page.netlify.app",
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/Tribute-Dr.AbdulQadeerKhan",
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

    {
        id: 6,
        title: "JS Technical Documentation",
        desc: "A technical documentation page covering JavaScript concepts. Features a sticky sidebar navigation and structured content sections — inspired by freeCodeCamp's documentation project.",
        image: '/project6.png', 
        category: 'HTML/CSS',
        bordColor: 'border-cyan-500/20',
        badgColor: 'bg-cyan-500',
        technolg: [
            { name: "HTML", class: 'bg-blue-500/20 border-blue-400/30 text-blue-200' },
            { name: "CSS",  class: 'bg-cyan-500/20 border-cyan-400/30 text-cyan-200' },
        ],
        links: [
            {
                name: "Live Demo",
                url: "https://your-docs-page.netlify.app",
                icon: EyeIcon,
                class: 'text-blue-400 hover:text-blue-300'
            },
            {
                name: "Code",
                url: "https://github.com/Ex-Noob/TechnicalDocumentationPage",
                icon: CodeBracketIcon,
                class: 'text-cyan-400 hover:text-cyan-300'
            },
        ]
    },

])
</script>

<style></style>