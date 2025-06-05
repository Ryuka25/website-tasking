<script setup lang="ts">
import { defineProps } from "vue";

const navbarStyle = {
  transparent: "bg-transparent text-white",
  light: "bg-white text-black",
};

const props = defineProps<{
  variant?: "transparent" | "light";
}>();
</script>

<template>
  <div
    :class="[
      navbarStyle[props.variant || 'transparent'],
      'transition-all duration-150 h-24 w-full text-center flex justify-center items-center font-bold uppercase',
    ]"
  >
    <Icon name="streamline-stickies-color:baby-cart-quality" />
    <span class="ml-2"> Navigation Bar </span>
  </div>
</template>
