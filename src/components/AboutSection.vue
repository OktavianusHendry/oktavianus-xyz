<template>
  <section class="text-white mt-18" id="about">
    <div class="absolute z-0 top-[93rem] inset-x-0 h-64 flex items-start">
      <div
        class="mt-20 h-24 w-64 bg-gradient-to-br from-primary via-secondary blur-2xl to-[#570cac] opacity-20"></div>
    </div>

    <div
      class="overflow-x-hidden md:grid md:grid-cols-2 gap-8 items-start py-8 px-4 xl:gap-16 sm:py-16 xl:px-16 z-1">
      <div data-aos="fade-right">
        <h2 class="text-4xl font-bold text-white text-left mb-8">
          My Education
        </h2>
        <div class="space-y-8 py-8">
          <div
            v-for="element in education"
            :key="element.id"
            class="flex items-center md:w-[80%] w-full rounded-xl bg-[#111a3e] shadow-lg border-[#1f1641]">
            <div class="w-1/4 p-4">
              <img
                src="https://img.icons8.com/ios-glyphs/60/ffffff/graduation-cap--v1.png"
                alt="education icon" />
            </div>
            <div class="w-3/4 pl-4">
              <h3
                class="text-2xl font-semibold uppercase text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">
                {{ element.school }}
              </h3>
              <p>{{ element.program }}</p>
              <p>{{ element.year }}</p>
            </div>
          </div>
        </div>
      </div>
      <div
        class="mt-4 md:mt-0 text-left flex flex-col z-10 h-full"
        data-aos="fade-left">
        <h2 class="text-4xl font-bold text-white md:text-center text-left mb-4">
          More
          <span
            class="text-transparent bg-clip-text bg-gradient-to-r from-primary to-secondary">
            About Me</span
          >
        </h2>
        <p class="text-base lg:text-lg mt-8 py-8">
          IT Student at Pradita University and graduated from Bangkit Academy
          2023 Batch 2 as a Mobile Development Cohort. I am interested in
          Application Development, Web Development, and Internet of Things. I
          have developed various skills through my learning experience.
          Dedicated to improving my skills and looking forward to developing and
          making use of my skills in the Mobile Development industry
        </p>
        <div class="grid grid-cols-3 gap-4 max-w-lg pt-8">
          <div
            class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
            <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">
              1 Year+
            </h3>
            <p class="text-sm sm:text-base text-gray-300">Web Development</p>
          </div>
          <div
            class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
            <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">
              5+
            </h3>
            <p class="text-sm sm:text-base text-gray-300">Organization</p>
          </div>
          <div
            class="text-center rounded-xl bg-[#111a3e] shadow-lg border border-[#1f1641] p-3">
            <h3 class="text-white font-bold text-xl sm:text-2xl lg:text-3xl">
              10+
            </h3>
            <p class="text-sm sm:text-base text-gray-300">Certification</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";
const education = ref([
  //ide sementara jadiin experience di webdev blabla
  {
    id: 1,
    school: "Pradita University",
    program: "Informatics",
    year: "2025",
  },
  {
    id: 2,
    school: "Bangkit Academy",
    program: "Mobile Development Cohort",
    year: "2023 Batch 2",
  },
]);
</script>
