<template>
    <section class="relative py-20 overflow-hidden" id="testimonials">
        <div class="relative z-10 max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">

            <!-- Section Header -->
            <div class="text-center mb-16" data-aos="fade-up">
                <h2 class="text-4xl md:text-5xl font-bold text-white mb-4">
                    Why Work
                    <span class="text-transparent bg-clip-text bg-linear-to-r from-blue-400 to-cyan-400">
                        With Me
                    </span>
                </h2>
                <p class="text-blue-200 text-lg">
                    What you get when you work with me
                </p>
            </div>

            <!-- Cards Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <div
                    v-for="(card, index) in reasons"
                    :key="card.id"
                    class="group bg-linear-to-br from-gray-800/50 to-blue-900/30 rounded-2xl p-6 border border-blue-500/20 backdrop-blur-sm hover:border-blue-400/50 transition-all duration-300 hover:-translate-y-1"
                    data-aos="fade-up"
                    :data-aos-delay="index * 100">

                    <!-- Icon -->
                    <div class="w-12 h-12 rounded-xl flex items-center justify-center mb-4"
                        :class="card.iconBg">
                        <component :is="card.icon" class="w-6 h-6" :class="card.iconColor" />
                    </div>

                    <!-- Content -->
                    <h3 class="text-white font-bold text-lg mb-2 group-hover:text-blue-400 transition-colors duration-300">
                        {{ card.title }}
                    </h3>
                    <p class="text-blue-100 text-sm leading-relaxed">
                        {{ card.desc }}
                    </p>

                </div>
            </div>

            <!-- Bottom CTA -->
            <div class="text-center mt-16" data-aos="fade-up">
                <p class="text-blue-200 text-lg mb-6">
                    Ready to start something together?
                </p>
                <button
                    @click="scrollToContact"
                    class="px-8 py-4 rounded-xl bg-linear-to-r from-blue-500 to-cyan-500 text-white font-semibold hover:shadow-lg hover:shadow-blue-500/25 transition-all duration-300 hover:scale-105 flex items-center gap-2 mx-auto">
                    <ChatBubbleLeftRightIcon class="w-5 h-5" />
                    Let's Talk
                </button>
            </div>

        </div>
    </section>
</template>

<script setup>
import {
    BoltIcon,
    ChatBubbleLeftRightIcon,
    CheckBadgeIcon,
    ClockIcon,
    CurrencyDollarIcon,
    ArrowPathIcon
} from '@heroicons/vue/16/solid';

const scrollToContact = () => {
    document.getElementById('contact')?.scrollIntoView({ behavior: 'smooth' });
};

const reasons = [
    {
        id: 1,
        icon: CheckBadgeIcon,
        iconBg: 'bg-blue-500/20 border border-blue-400/30',
        iconColor: 'text-blue-400',
        title: 'Honest About My Skills',
        desc: "I only take on work I can genuinely deliver. No overpromising — you always know exactly what you're getting."
    },
    {
        id: 2,
        icon: BoltIcon,
        iconBg: 'bg-cyan-500/20 border border-cyan-400/30',
        iconColor: 'text-cyan-400',
        title: 'Fast & Responsive',
        desc: 'I respond quickly and keep you updated throughout the project. No ghosting, no long silences.'
    },
    {
        id: 3,
        icon: ArrowPathIcon,
        iconBg: 'bg-blue-500/20 border border-blue-400/30',
        iconColor: 'text-blue-400',
        title: 'Revisions Until You\'re Happy',
        desc: "I don't disappear after delivery. If something needs fixing, I fix it — your satisfaction matters."
    },
    {
        id: 4,
        icon: CurrencyDollarIcon,
        iconBg: 'bg-cyan-500/20 border border-cyan-400/30',
        iconColor: 'text-cyan-400',
        title: 'Affordable Rates',
        desc: 'Fair pricing for quality work. I offer competitive rates because I want to build a strong portfolio too.'
    },
    {
        id: 5,
        icon: ClockIcon,
        iconBg: 'bg-blue-500/20 border border-blue-400/30',
        iconColor: 'text-blue-400',
        title: 'On-Time Delivery',
        desc: 'Deadlines are serious to me. I plan my work properly so your project is delivered when promised.'
    },
    {
        id: 6,
        icon: ChatBubbleLeftRightIcon,
        iconBg: 'bg-cyan-500/20 border border-cyan-400/30',
        iconColor: 'text-cyan-400',
        title: 'Clear Communication',
        desc: 'No confusing tech talk. I explain everything simply and keep the whole process easy for you.'
    },
]
</script>

<style></style>