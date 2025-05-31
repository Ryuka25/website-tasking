<script setup lang="ts">
import type { LandingPage } from "~/types";
import landingPagesData from "~/data/landing-pages.json";

const landingPages = landingPagesData as LandingPage[];
</script>

<template>
  <div class="bg-white dark">
    <div class="w-full max-w-6xl mx-auto">
      <h1
        class="text-balance text-5xl font-semibold tracking-tight text-gray-900 sm:text-7xl"
      >
        Landing pages
      </h1>
      <div class="w-4/5 gap-4 flex flex-row mt-8">
        <div v-for="(landingPage, index) in landingPages" :key="index">
          <NuxtLink :href="landingPage.url">
            <div class="bg-gray-200 aspect-video w-80 rounded-md" />
            <div class="">
              {{ landingPage.title }}
            </div>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>
