<template>
  <section
    class="bg-[#FAFAFA] min-h-screen flex flex-col justify-center items-center"
  >
    <header class="text-[2.2rem]">
      <h1 class="font-light">Reliable, efficient delivery</h1>
      <h2 class="font-semibold-bold">Powered by Technology</h2>
    </header>
    <main>
      <p class="text-[0.938rem]">
        Our Artificial Intelligence powered tools use millions of project data
        points to ensure that your project is successful
      </p>
      <base-card
        v-for="(item, index) in cards"
        :key="index"
        :border-color="item.borderColor"
        :img-src="item.imgSrc"
      ></base-card>
    </main>
  </section>
</template>

<script setup>
import BaseCard from "./components/BaseCard.vue";

const cards = [
  {
    heading: "Supervisor",
    description: "Monitors activity to identify project roadblocks",
    imgSrc: "../assets/images/icon-supervisor.svg",
    borderColor: "border-[#45D3D3]",
  },
  {
    heading: "Team Builder",
    description: "Builds teams to take on any project",
    imgSrc: "../assets/images/icon-team-builder.svg",
    borderColor: "border-[#EA5353]",
  },
  {
    heading: "Karma",
    description: "Regularly evaluates our talent to ensure quality",
    imgSrc: "../assets/images/icon-karma.svg",
    borderColor: "border-[#FCAF4A]",
  },
  {
    heading: "Calculator",
    description: "Uses data to provide insights on projects",
    imgSrc: "../assets/images/icon-calculator.svg",
    borderColor: "border-[#549EF2]",
  },
];
</script>
