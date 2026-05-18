<template>
    <footer class="relative bg-gray-900/80 border-t border-blue-500/20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 py-12">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">

                <!-- Brand -->
                <div class="md:col-span-2">
                    <div class="text-2xl font-bold bg-linear-to-r from-blue-400 to-cyan-400 bg-clip-text text-transparent mb-4">
                        Ibti.dev
                    </div>
                    <p class="text-blue-200 text-sm leading-relaxed max-w-md">
                        Self-taught front-end developer from Karachi, Pakistan. I build clean, responsive websites and take on real freelance projects. Always learning, always building.
                    </p>
                    <div class="flex gap-4 mt-6">

                        <!-- Email -->
                        <a href="mailto:ibtihaj.dev@gmail.com"
                            title="Email"
                            class="p-2 bg-blue-500/20 border border-blue-400/30 rounded-lg text-blue-400 hover:bg-blue-500/30 transition-all">
                            <EnvelopeIcon class="w-5 h-5" />
                        </a>

                        <!-- GitHub -->
                        <a href="https://github.com/Ex-Noob"
                            target="_blank" rel="noopener noreferrer"
                            title="GitHub"
                            class="p-2 bg-gray-500/20 border border-gray-400/30 rounded-lg text-gray-400 hover:bg-gray-500/30 transition-all">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M12 0C5.37 0 0 5.37 0 12c0 5.3 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.387-1.333-1.756-1.333-1.756-1.09-.745.083-.729.083-.729 1.205.085 1.84 1.237 1.84 1.237 1.07 1.834 2.807 1.304 3.492.997.108-.775.418-1.305.762-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.605-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 21.795 24 17.295 24 12c0-6.63-5.37-12-12-12z"/>
                            </svg>
                        </a>

                        <!-- LinkedIn -->
                        <a href="https://www.linkedin.com/in/muhammad-ibtihaj-dev/"
                            target="_blank" rel="noopener noreferrer"
                            title="LinkedIn"
                            class="p-2 bg-blue-600/20 border border-blue-500/30 rounded-lg text-blue-400 hover:bg-blue-600/30 transition-all">
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
                            </svg>
                        </a>

                        <!-- WhatsApp -->
                        <a href="https://wa.me/923073486980"
                            target="_blank" rel="noopener noreferrer"
                            title="WhatsApp"
                            class="p-2 bg-green-500/20 border border-green-400/30 rounded-lg text-green-400 hover:bg-green-500/30 transition-all">
                            
                            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/>
                            </svg>
                        </a>

                    </div>
                </div>

                <!-- Quick Links -->
                <div>
                    <h3 class="text-white font-semibold mb-4">Quick Links</h3>
                    <ul class="space-y-2">
                        <li v-for="link in quickLinks" :key="link.name">
                            <a :href="link.href"
                                class="text-blue-200 hover:text-blue-400 text-sm transition-colors duration-300">
                                {{ link.name }}
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- Services -->
                <div>
                    <h3 class="text-white font-semibold mb-4">Services</h3>
                    <ul class="space-y-2">
                        <li v-for="service in services" :key="service">
                            <span class="text-blue-200 text-sm">{{ service }}</span>
                        </li>
                    </ul>
                </div>

            </div>

            <!-- Bottom Bar -->
            <div class="border-t border-blue-500/20 mt-8 pt-8 flex flex-col md:flex-row justify-between items-center gap-4">
                <p class="text-blue-300 text-sm">
                    © 2026 Ibti.dev — Built with Vue.js & Tailwind CSS
                </p>
                <p class="text-blue-400 text-sm italic">
                    "Every expert was once a beginner." 🚀
                </p>
            </div>

        </div>
    </footer>
</template>

<script setup>
import {
    EnvelopeIcon,
} from '@heroicons/vue/24/outline';

const quickLinks = [
    { name: "Home",         href: "#hero" },
    { name: "About",        href: "#about" },
    { name: "Skills",       href: "#skills" },
    { name: "Services",     href: "#services" },
    { name: "Projects",     href: "#projects" },
    { name: "Contact",      href: "#contact" },
]

const services = [
    'Front-End Development',
    'Web Design',
    'Visual Content Design',
    'Digital Marketing',
    'Content Creation & Photo Editing',
    'Data Entry & Management',
]
</script>

<style></style>