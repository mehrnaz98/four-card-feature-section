<template>
  <div
    class="flex flex-col bg-white shadow-lg max-w-[21.5rem] rounded-lg p-7 border-t-4"
    :class="borderColor"
  >
    <h2 class="font-bold text-[1.4rem] text-[#4C4E61]">
      <slot name="heading">Default Heading</slot>
    </h2>
    <p class="text-[0.875rem] text-[#A3A5AE] pt-3">
      <slot name="description">Default description text</slot>
    </p>
    <div class="flex justify-end">
      <img
        src="../assets/images/icon-supervisor.svg"
        alt=""
        class="pt-8 max-w-16"
      />
    </div>
  </div>
</template>
