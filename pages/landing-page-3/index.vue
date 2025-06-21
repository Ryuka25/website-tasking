<template>
  <div class="w-full min-h-screen flex justify-center items-center antialiased">
    <div class="max-w-5xl w-full h-ful mx-auto flex">
      <div class="w-1/2 flex flex-col justify-center gap-7">
        <div class="text-4xl text-pretty font-bold">
          Impactfull header goes there to show how much it's good
        </div>
        <div class="w-1/2">
          Additionnal Paragraph to explain what's the matter and why it's not
          possible to implement everything
        </div>
        <div>
          <button
            class="bg-black hover:bg-black/80 text-white px-8 py-2 rounded-lg"
          >
            Click me
          </button>
        </div>
      </div>
      <div class="w-1/2 flex justify-end items-center">
        <img
          src="/assets/landing-page-3/hero-image.webp"
          alt="hero"
          class="w-3/4 rounded-lg"
        />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Inter:ital,opsz,wght@0,14..32,100..900;1,14..32,100..900&display=swap");

* {
  font-family: "Inter";
}
</style>
