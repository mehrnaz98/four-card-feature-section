<template>
  <section
    class="bg-[#FAFAFA] min-h-screen flex flex-col justify-center items-center p-6"
  >
    <header class="text-[2rem]">
      <h1 class="poppins-extralight text-[#4C4E61]">
        Reliable, efficient delivery
      </h1>
      <h2 class="poppins-semibold text-[#4C4E61]">Powered by Technology</h2>
    </header>
    <main class="flex flex-col justify-center items-center">
      <div class="w-[30rem]">
        <p
          class="poppins-regular text-[#A3A5AE] text-[0.938rem] text-center pt-4"
        >
          Our Artificial Intelligence powered tools use millions of project data
          points to ensure that your project is successful
        </p>
      </div>
      <div class="grid-container mt-12">
        <base-card
          v-for="(item, index) in cards"
          :key="index"
          :border-color="item.borderColor"
          :img-src="item.imgSrc"
          :class="item.id"
        >
          <template #heading>{{ item.heading }}</template>
          <template #description>{{ item.description }}</template>
        </base-card>
      </div>
    </main>
  </section>
</template>

<script setup>
import BaseCard from "./components/BaseCard.vue";
import iconSupervisor from "./assets/images/icon-supervisor.svg";
import iconTeamBuilder from "./assets/images/icon-team-builder.svg";
import iconKarma from "./assets/images/icon-karma.svg";
import iconCalculator from "./assets/images/icon-calculator.svg";

const cards = [
  {
    id: "item1",
    heading: "Supervisor",
    description: "Monitors activity to identify project roadblocks",
    imgSrc: iconSupervisor,
    borderColor: "border-[#45D3D3]",
  },
  {
    id: "item2",
    heading: "Team Builder",
    description: "Builds teams to take on any project",
    imgSrc: iconTeamBuilder,
    borderColor: "border-[#EA5353]",
  },
  {
    id: "item3",
    heading: "Karma",
    description: "Regularly evaluates our talent to ensure quality",
    imgSrc: iconKarma,
    borderColor: "border-[#FCAF4A]",
  },
  {
    id: "item4",
    heading: "Calculator",
    description: "Uses data to provide insights on projects",
    imgSrc: iconCalculator,
    borderColor: "border-[#549EF2]",
  },
];
</script>
