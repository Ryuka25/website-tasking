<script setup lang="ts">
import NavBar from "./nav-bar.vue";

const navbarVariant = ref<"transparent" | "light">("transparent");

onMounted(() => {
  document.addEventListener("scroll", () => {
    if (window.scrollY > 5) {
      navbarVariant.value = "light";
    } else {
      navbarVariant.value = "transparent";
    }
  });
});
</script>

<template>
  <div class="relative">
    <div id="navbar" class="fixed t-0 l-0 w-full z-10">
      <NavBar :variant="navbarVariant" />
      <!-- <NavBar variant="transparent" /> -->
    </div>
    <div class="h-screen">
      <NuxtImg
        src="/assets/lading-page-2/bg.jpg"
        alt="Example Image"
        class="h-full object-cover bg-black brightness-75"
      />
    </div>
    <div class="w-full h-screen">
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
