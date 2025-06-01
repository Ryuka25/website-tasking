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

    <section class="bg-blue-50 text-center">
      <div class="max-w-6xl mx-auto px-7 py-10">
        <div class="mb-14">
          <p class="text-blue-600 text-lg">Features</p>
          <h1 class="font-bold text-4xl">Our Special Features</h1>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">
          <div class="bg-white rounded-md py-6 px-2">
            <div
              class="bg-blue-200 text-blue-500 w-16 h-16 rounded-md mx-auto flex justify-center items-center text-3xl"
            >
              <Icon name="lucide:user" />
            </div>
            <h2 class="font-bold text-2xl my-3">User Friendly</h2>
            <p class="max-w-md mx-auto text-gray-400">
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veniam,
              velit.
            </p>
          </div>
          <div class="bg-white rounded-md text-center py-6 px-2">
            <div
              class="bg-blue-200 text-blue-500 w-16 h-16 rounded-md mx-auto flex justify-center items-center text-3xl"
            >
              <Icon name="lucide:shield" />
            </div>
            <h2 class="font-bold text-2xl my-3">Trusted</h2>
            <p class="max-w-md mx-auto text-gray-400">
              Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit,
              deserunt?
            </p>
          </div>
          <div class="bg-white rounded-md text-center py-6 px-2">
            <div
              class="bg-blue-200 text-blue-500 w-16 h-16 rounded-md mx-auto flex justify-center items-center text-3xl"
            >
              <Icon name="lucide:sticky-note" />
            </div>
            <h2 class="font-bold text-2xl my-3">Flexible</h2>
            <p class="max-w-md mx-auto text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta,
              officiis!
            </p>
          </div>
          <div class="bg-white rounded-md text-center py-6 px-2">
            <div
              class="bg-blue-200 text-blue-500 w-16 h-16 rounded-md mx-auto flex justify-center items-center text-3xl"
            >
              <Icon name="lucide:percent" />
            </div>
            <h2 class="font-bold text-2xl my-3">100% Free</h2>
            <p class="max-w-md mx-auto text-gray-400">
              Lorem ipsum dolor sit amet, consectetur adipisicing elit.
              Eligendi, autem.
            </p>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-slate-50">
      <div class="max-w-6xl mx-auto px-7 py-10">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-7 items-center mb-12">
          <NuxtImg src="/assets/landing-page-1/img2.svg" />
          <div>
            <p class="text-blue-600 mb-4 text-lg">Superiority</p>
            <h1 class="font-bold text-4xl">
              Smart System &amp; Friendly Design
            </h1>
            <p class="max-w-md my-6 text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Totam
              vero doloribus eius aspernatur dolorum rerum repellendus, qui modi
              magni iusto!
            </p>
            <a
              href="#"
              class="bg-blue-700 hover:bg-blue-800 transition-colors text-white py-3 px-7 rounded-md mr-4 mt-1 inline-block text-lg"
            >
              Learn More
            </a>
          </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-7 items-center mt-12">
          <div class="order-2 md:order-1">
            <p class="text-blue-600 mb-4 text-lg">How it works</p>
            <h1 class="font-bold text-4xl">
              How It Works? <br />
              We Have Three Options
            </h1>
            <p class="max-w-md my-6 text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Temporibus voluptatum repellat cum nostrum minima quam totam minus
              magnam, exercitationem porro!
            </p>
            <a
              href="#"
              class="bg-blue-700 hover:bg-blue-800 transition-colors text-white py-3 px-7 rounded-md mr-4 mt-1 inline-block text-lg"
            >
              Learn More
            </a>
          </div>
          <NuxtImg
            src="/assets/landing-page-1/img3.svg"
            class="order-1 md:order-2"
          />
        </div>
      </div>
    </section>
  </div>
</template>
