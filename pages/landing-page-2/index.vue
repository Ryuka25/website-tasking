<script setup lang="ts"></script>

<template>
  <div class="relative">
    <div id="navbar" class="fixed t-0 l-0 w-full z-10">
      <div
        class="h-24 w-full text-center flex justify-center items-center font-bold uppercase text-white"
      >
        <Icon name="streamline-stickies-color:baby-cart-quality" />
        <span class="ml-2"> Navigation Bar </span>
      </div>
    </div>
    <div class="h-screen">
      <NuxtImg
        src="/assets/lading-page-2/bg.jpg"
        alt="Example Image"
        class="h-full object-cover bg-black brightness-75"
      />
    </div>
    <div class="w-full h-[1000px]">
      <div
        class="w-full h-full bg-slate-200 flex justify-center items-center p-4 text-slate-700"
      >
        <Icon
          name="streamline-stickies-color:baby-cart-quality"
          class="size-96"
        />
      </div>
    </div>
  </div>
</template>
