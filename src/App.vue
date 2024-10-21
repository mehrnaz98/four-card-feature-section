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
      <BaseCard />
    </main>
  </section>
</template>

<script setup>
import BaseCard from "./components/BaseCard.vue";
</script>
