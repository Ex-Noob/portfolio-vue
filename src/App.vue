<template>
  <div class="min-h-screen bg-linear-to-br from-gray-900 via-blue-900 to-gray-900">
    <Navbar />
    <Hero />
    <Services />
    <About />
    <ExperienceSkills />
    <Projects />
    <Contact />
    <Testimonials />
    <Footer />
  </div>
</template>
<script>
import AOS from "aos";
import "aos/dist/aos.css";
import Hero from "./components/Hero.vue";
import Navbar from "./components/Navbar.vue";


import { ref, nextTick, onMounted } from "vue";
import Services from "./components/Services.vue";
import About from "./components/About.vue";
import ExperienceSkills from "./components/ExperienceSkills.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Testimonials from "./components/testimonials.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Navbar,
    Hero,
    Services,
    About,
    ExperienceSkills,
    Projects,
    Contact,
    Testimonials,
    Footer,

  },
  setup() {
    const loading = ref(true);

    onMounted(async () => {
      await nextTick();

      AOS.init({
        duration: 800,
        once: false,
        offset: 100,
        easing: "ease-in-out",
      });
      setTimeout(() => {
        loading.value = false;
      }, 800);
    });
    return { loading };
  }
}
</script>
