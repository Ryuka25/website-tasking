<script setup lang="ts"></script>
<template>
  <div>
    <nav class="fixed w-full bg-white drop-shadow-md">
      <div class="max-w-6xl flex justify-between items-center mx-auto p-7">
        <a href="#" class="font-bold text-3xl">Tasking</a>
        <ul
          id="navbar-menu"
          class="bg-white flex justify-between items-center flex-col gap-5 text-gray-400 absolute overflow-y-scroll w-full left-0 top-20 px-6 transition-all duration-500 ease-out h-0 md:static md:flex-row md:h-auto md-top-auto md:overflow-auto md:justify-center md:w-fit"
        >
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Member</a></li>
          <li><a href="#">Entreprise</a></li>
          <li>
            <a
              href="#"
              class="bg-blue-700 transition-colors hover:bg-blue-800 text-white py-2 px-7 rounded-md block md:hidden"
            >
              Sign up
            </a>
          </li>
        </ul>
        <a
          href="#"
          class="bg-blue-700 transition-colors hover:bg-blue-800 text-white py-2 px-7 rounded-md hidden md:block"
        >
          Sign up
        </a>
        <button id="menu-btn" class="md:hidden">
          <Icon class="text-2xl" name="lucide:menu" />
        </button>
      </div>
    </nav>

    <header class="min-h-screen flex justify-center items-center pt-36 pb-7">
      <div
        class="grid grid-cols-1 md:grid-cols-2 items-center max-w-6xl mx-auto px-7"
      >
        <div class="mb-10 md:mb-0">
          <h1 class="text-5xl md:text-6xl lg:text-7xl xl:text-8xl">
            Manage <br />
            your
            <span class="font-bold">tasks</span>
            quickly
          </h1>
          <p class="mb-5 mt-7 max-w-md text-gray-400">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Provident
            nesciunt dicta consequuntur earum culpa voluptatibus!
          </p>
          <a
            href="#"
            class="bg-blue-700 hover:bg-blue-800 transition-colors text-white py-3 px-7 rounded-md mr-4 mt-1 inline-block text-lg"
          >
            Get Started
          </a>
          <a href="#" class="font-bold">Learn More</a>
        </div>
        <NuxtImg src="/assets/landing-page-1/img1.svg" />
      </div>
    </header>
  </div>
</template>
