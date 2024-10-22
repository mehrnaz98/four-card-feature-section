<template>
  <div
    class="flex flex-col bg-white shadow-xl max-w-[20rem] rounded-lg p-7 border-t-4"
    :style="{ borderColor: borderColor }"
  >
    <h2 class="poppins-semibold text-[1.1rem] text-[#4C4E61]">
      <slot name="heading">Default Heading</slot>
    </h2>
    <p class="poppins-regular text-[0.8rem] text-[#A3A5AE] pt-2">
      <slot name="description">Default description text</slot>
    </p>
    <div class="flex justify-end">
      <img :src="imgSrc" alt="" class="pt-8 max-w-14" />
    </div>
  </div>
</template>

<script setup>
defineProps({
  borderColor: {
    type: String,
    default: "#45D3D3",
  },
  imgSrc: {
    type: String,
    default: "../assets/images/icon-supervisor.svg",
  },
});
</script>
