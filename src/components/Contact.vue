<template>
    <section class="relative py-20 overflow-hidden" id="contact">
        <div class="relative z-10 max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16" data-aos="fade-up">
                <h2 class="text-4xl md:text-5xl font-bold text-white mb-4">
                    Get In <span class="text-transparent bg-clip-text bg-linear-to-r from-blue-400 to-cyan-400">
                        Touch</span>
                </h2>
                <p class="text-blue-200 text-lg">
                    Let's work together on your next project
                </p>
            </div>

            <div class="grid lg:grid-cols-2 gap-12">

                <!-- Contact Info -->
                <div data-aos="fade-right">
                    <h3 class="text-2xl font-bold text-white mb-6">Contact Information</h3>
                    <div class="space-y-6">

                        <!-- Email -->
                        <div class="flex items-center gap-4">
                            <EnvelopeIcon class="w-6 h-6 text-blue-400 shrink-0" />
                            <div>
                                <p class="text-white font-semibold">Email</p>
                                <a href="mailto:ibtihajgo@gmail.com"
                                    class="text-blue-200 hover:text-blue-400 transition-colors duration-300">
                                    ibtihajgo@gmail.com
                                </a>
                            </div>
                        </div>

                        <!-- Location -->
                        <div class="flex items-center gap-4">
                            <MapPinIcon class="w-6 h-6 text-blue-400 shrink-0" />
                            <div>
                                <p class="text-white font-semibold">Location</p>
                                <p class="text-blue-200">Karachi, Pakistan</p>
                            </div>
                        </div>

                        <!-- Availability -->
                        <div class="flex items-center gap-4">
                            <CheckCircleIcon class="w-6 h-6 text-green-400 shrink-0" />
                            <div>
                                <p class="text-white font-semibold">Availability</p>
                                <p class="text-green-400 font-medium">Open to freelance projects</p>
                            </div>
                        </div>

                    </div>

                    <!-- Social Links -->
                    <div class="mt-8">
                        <h4 class="text-lg font-bold text-white mb-4">Find Me On</h4>
                        <div class="flex gap-4">

                            <!-- GitHub -->
                            <a href="https://github.com/Ex-Noob"
                                target="_blank" rel="noopener noreferrer"
                                class="group p-3 bg-gray-500/20 border border-gray-400/30 rounded-xl text-gray-400 hover:bg-gray-500/30 hover:text-white hover:border-gray-400/60 transition-all duration-300"
                                title="GitHub">
                                <!-- GitHub SVG icon -->
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M12 0C5.37 0 0 5.37 0 12c0 5.3 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.387-1.333-1.756-1.333-1.756-1.09-.745.083-.729.083-.729 1.205.085 1.84 1.237 1.84 1.237 1.07 1.834 2.807 1.304 3.492.997.108-.775.418-1.305.762-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.605-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 21.795 24 17.295 24 12c0-6.63-5.37-12-12-12z"/>
                                </svg>
                            </a>

                            <!-- LinkedIn -->
                            <a href="https://www.linkedin.com/in/muhammad-ibtihaj-dev/"
                                target="_blank" rel="noopener noreferrer"
                                class="group p-3 bg-blue-600/20 border border-blue-500/30 rounded-xl text-blue-400 hover:bg-blue-600/30 hover:text-blue-300 hover:border-blue-400/60 transition-all duration-300"
                                title="LinkedIn">
                                <!-- LinkedIn SVG icon -->
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 01-2.063-2.065 2.064 2.064 0 112.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
                                </svg>
                            </a>

                            <!-- WhatsApp -->
                            <a href="https://wa.me/923073486980"
                                target="_blank" rel="noopener noreferrer"
                                class="group p-3 bg-green-500/20 border border-green-400/30 rounded-xl text-green-400 hover:bg-green-500/30 hover:text-green-300 hover:border-green-400/60 transition-all duration-300"
                                title="WhatsApp">
                                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                                    <path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/>
                                </svg>
                            </a>

                        </div>
                    </div>
                </div>

                <!-- Contact Form -->
                <div data-aos="fade-left">

                    <!-- Success Message -->
                    <div v-if="formStatus === 'success'"
                        class="mb-6 p-4 bg-green-500/10 border border-green-400/30 rounded-xl text-green-400 text-sm font-medium">
                        ✅ Message sent! I'll get back to you soon.
                    </div>

                    <!-- Error Message -->
                    <div v-if="formStatus === 'error'"
                        class="mb-6 p-4 bg-red-500/10 border border-red-400/30 rounded-xl text-red-400 text-sm font-medium">
                        ❌ Something went wrong. Please try again or email me directly.
                    </div>

                    <form @submit.prevent="sendEmail" class="space-y-5">

                        <!-- Name & Email row -->
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-5">
                            <div>
                                <label class="text-white text-sm font-medium mb-2 block">Name</label>
                                <input v-model="form.name" type="text" placeholder="Your name"
                                    class="w-full bg-gray-800/50 border border-blue-500/30 rounded-xl px-4 py-3 text-white placeholder-blue-300/50 focus:border-blue-400 focus:outline-none transition-all duration-300" />
                                <p v-if="errors.name" class="text-red-400 text-xs mt-1">{{ errors.name }}</p>
                            </div>
                            <div>
                                <label class="text-white text-sm font-medium mb-2 block">Email</label>
                                <input v-model="form.email" type="email" placeholder="your@email.com"
                                    class="w-full bg-gray-800/50 border border-blue-500/30 rounded-xl px-4 py-3 text-white placeholder-blue-300/50 focus:border-blue-400 focus:outline-none transition-all duration-300" />
                                <p v-if="errors.email" class="text-red-400 text-xs mt-1">{{ errors.email }}</p>
                            </div>
                        </div>

                        <!-- Subject -->
                        <div>
                            <label class="text-white text-sm font-medium mb-2 block">Subject</label>
                            <input v-model="form.subject" type="text" placeholder="What's this about?"
                                class="w-full bg-gray-800/50 border border-blue-500/30 rounded-xl px-4 py-3 text-white placeholder-blue-300/50 focus:border-blue-400 focus:outline-none transition-all duration-300" />
                            <p v-if="errors.subject" class="text-red-400 text-xs mt-1">{{ errors.subject }}</p>
                        </div>

                        <!-- Message -->
                        <div>
                            <label class="text-white text-sm font-medium mb-2 block">Message</label>
                            <textarea v-model="form.message" rows="4" placeholder="Tell me about your project..."
                                class="w-full bg-gray-800/50 border border-blue-500/30 rounded-xl px-4 py-3 text-white placeholder-blue-300/50 focus:border-blue-400 focus:outline-none transition-all duration-300 resize-none">
                            </textarea>
                            <p v-if="errors.message" class="text-red-400 text-xs mt-1">{{ errors.message }}</p>
                        </div>

                        <!-- Submit Button -->
                        <button type="submit" :disabled="isSending"
                            class="w-full bg-linear-to-r from-blue-500 to-cyan-500 text-white font-semibold py-3 rounded-xl hover:shadow-lg hover:shadow-blue-500/25 transition-all duration-300 hover:scale-[1.02] disabled:opacity-60 disabled:cursor-not-allowed disabled:hover:scale-100">
                            {{ isSending ? 'Sending...' : 'Send Message' }}
                        </button>

                    </form>
                </div>

            </div>
        </div>
    </section>
</template>

<script setup>
import {
    EnvelopeIcon,
    MapPinIcon,
    CheckCircleIcon
} from '@heroicons/vue/16/solid';
import { ref, reactive } from 'vue';
import emailjs from '@emailjs/browser';


const EMAILJS_SERVICE_ID  = 'service_wa2vtov';   
const EMAILJS_TEMPLATE_ID = 'template_jjlxsct';  
const EMAILJS_PUBLIC_KEY  = 'tG0u79OGFloqf6JWZ';   



const form = reactive({
    name: '',
    email: '',
    subject: '',
    message: ''
});

const errors = reactive({
    name: '',
    email: '',
    subject: '',
    message: ''
});

const isSending = ref(false);
const formStatus = ref(''); // 'success' | 'error' | ''

const validate = () => {
    let valid = true;
    errors.name    = '';
    errors.email   = '';
    errors.subject = '';
    errors.message = '';

    if (!form.name.trim()) {
        errors.name = 'Name is required.';
        valid = false;
    }
    if (!form.email.trim()) {
        errors.email = 'Email is required.';
        valid = false;
    } else if (!/^\S+@\S+\.\S+$/.test(form.email)) {
        errors.email = 'Please enter a valid email.';
        valid = false;
    }
    if (!form.subject.trim()) {
        errors.subject = 'Subject is required.';
        valid = false;
    }
    if (!form.message.trim()) {
        errors.message = 'Message is required.';
        valid = false;
    }
    return valid;
};

const sendEmail = async () => {
    if (!validate()) return;

    isSending.value  = true;
    formStatus.value = '';

    try {
        await emailjs.send(
            EMAILJS_SERVICE_ID,
            EMAILJS_TEMPLATE_ID,
            {
                from_name:  form.name,
                from_email: form.email,
                subject:    form.subject,
                message:    form.message,
            },
            EMAILJS_PUBLIC_KEY
        );

        formStatus.value = 'success';
        form.name    = '';
        form.email   = '';
        form.subject = '';
        form.message = '';

    } catch (error) {
        console.error('EmailJS error:', error);
        formStatus.value = 'error';
    } finally {
        isSending.value = false;
    }
};
</script>

<style></style>