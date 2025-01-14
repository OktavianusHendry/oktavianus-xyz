<template>
  <div class="bg-[#111827] min-h-screen">
    <NavBar />
    <HeroSection />
    <ServicesSection />
    <AboutSection />
    <SkillsSection />
    <LatestProjectSection />
    <ContactSection />
    <FooterSection />
  </div>
</template>

<script setup>
import { defineAsyncComponent } from "vue";
// import HeroSection from "@/components/HeroSection.vue";
const NavBar = defineAsyncComponent(() => import("@/components/NavBar.vue"));
const HeroSection = defineAsyncComponent(() =>
  import("@/components/HeroSection.vue")
);
const ServicesSection = defineAsyncComponent(() =>
  import("@/components/ServicesSection.vue")
);
const AboutSection = defineAsyncComponent(() =>
  import("@/components/AboutSection.vue")
);
const SkillsSection = defineAsyncComponent(() =>
  import("@/components/SkillsSection.vue")
);
const LatestProjectSection = defineAsyncComponent(() =>
  import("@/components/LatestProjects.vue")
);
const ContactSection = defineAsyncComponent(() =>
  import("@/components/ContactSection.vue")
);
const FooterSection = defineAsyncComponent(() =>
  import("@/components/FooterSection.vue")
);
</script>
