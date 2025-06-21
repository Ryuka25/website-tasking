<script setup lang="ts">
import type { LandingPage } from "~/types";
import landingPagesData from "~/data/landing-pages.json";
import { Icon } from "#components";

const landingPages = landingPagesData as LandingPage[];

const onDescriptionCopy = (e: Event, description: string) => {
  e.preventDefault();
  navigator.clipboard
    .writeText(description)
    .then(() => {
      alert("Description copied to clipboard!");
    })
    .catch((error) => {
      console.error("Failed to copy text: ", error);
    });
};
</script>

<template>
  <div class="bg-white dark">
    <div class="max-w-6xl flex flex-col mx-auto p-7">
      <h1
        class="text-balance text-5xl font-semibold tracking-tight text-gray-900 sm:text-7xl"
      >
        Landing pages
      </h1>
      <div class="mt-8 w-full gap-4 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3">
        <div v-for="(landingPage, index) in landingPages" :key="index">
          <NuxtLink :href="landingPage.url">
            <NuxtImg
              :src="landingPage.image"
              class="bg-gray-200 aspect-video w-80 rounded-md"
            />
            <div class="font-bold mt-4">
              {{ landingPage.title }}
            </div>
            <div
              v-if="landingPage.description"
              class="text-slate-400 text-sm flex items-center gap-2"
            >
              <p>{{ landingPage.description }}</p>
              <Icon
                name="lucide:copy"
                class="hover:text-slate-700"
                @click="(e) => onDescriptionCopy(e, landingPage.description)"
              />
            </div>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>
