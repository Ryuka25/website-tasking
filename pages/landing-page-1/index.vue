<script setup lang="ts">
onMounted(() => {
  // Get elements for the mobile menu toggle
  const menu = document.getElementById("navbar-menu");
  const menuBtn = document.getElementById("menu-btn");

  // Add click event to menu btn
  menuBtn?.addEventListener("click", () => {
    // Toggle opened menu height
    if (menu) {
      menu.classList.toggle("h-52");
      // Toogle padding
      menu.classList.toggle("py-6");
      // Toogle closed menu height
      menu.classList.toggle("h-0");
    }
  });
});
</script>
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
    <section class="bg-white">
      <div class="max-w-6xl mx-auto px-7 py-10">
        <div class="mb-14 text-center">
          <p class="text-blue-600 text-lg">Articles</p>
          <h1 class="font-bold text-4xl">Articles From Tasking</h1>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
          <div class="border border-gray-200 rounded-lg p-4">
            <NuxtImg src="/assets/landing-page-1/blog1.jpg" class="mb-4" />
            <p class="text-gray-400 text-lg">Technology</p>
            <h2 class="text-2xl font-bold my-4">
              Bradford assay is an addition to comassie...
            </h2>
            <a
              href="#"
              class="flex justify-start items-center gap-4 hover:text-blue-600 transition-colors mb-2"
            >
              <span class="font-bold">Read More</span>
              <Icon name="lucide:arrow-right" class="text-blue-600" />
            </a>
          </div>
          <div class="border border-gray-200 rounded-lg p-4">
            <NuxtImg src="/assets/landing-page-1/blog2.jpg" class="mb-4" />
            <p class="text-gray-400 text-lg">Real Estate</p>
            <h2 class="text-2xl font-bold my-4">
              New economy, Real estate investment will be...
            </h2>
            <a
              href="#"
              class="flex justify-start items-center gap-4 hover:text-blue-600 transition-colors mb-2"
            >
              <span class="font-bold">Read More</span>
              <Icon name="lucide:arrow-right" class="text-blue-600" />
            </a>
          </div>
          <div class="border border-gray-200 rounded-lg p-4">
            <NuxtImg src="/assets/landing-page-1/blog3.jpg" class="mb-4" />
            <p class="text-gray-400 text-lg">Technology</p>
            <h2 class="text-2xl font-bold my-4">
              Revenue is targeted to increase by 20%...
            </h2>
            <a
              href="#"
              class="flex justify-start items-center gap-4 hover:text-blue-600 transition-colors mb-2"
            >
              <span class="font-bold">Read More</span>
              <Icon name="lucide:arrow-right" class="text-blue-600" />
            </a>
          </div>
        </div>
      </div>
    </section>
    <section class="bg-blue-50">
      <div class="max-w-6xl mx-auto px-7 py-10">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-7 items-center mb-12">
          <NuxtImg src="/assets/landing-page-1/img4.svg" />
          <div>
            <p class="text-blue-600 mb-4 text-lg">Download</p>
            <h1 class="font-bold text-4xl">Download Tasking On Your Device</h1>
            <p class="max-w-md my-6 text-gray-400">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsam
              inventore, totam mollitia veniam dicta suscipit cumque vero
              reiciendis architecto! Et!
            </p>
            <div class="flex justify-start items-center gap-4">
              <a href="#">
                <NuxtImg
                  src="/assets/landing-page-1/app-store-button.png"
                  class="h-12"
                />
              </a>
              <a href="#">
                <NuxtImg
                  src="/assets/landing-page-1/playstore-button.png"
                  class="h-12"
                />
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>

    <footer class="bg-indigo-800 text-white">
      <div
        class="max-w-6xl mx-auto px-7 py-10 grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12 lg:justify-items-center7"
      >
        <div>
          <h2 class="font-bold text-3xl">Tasking</h2>
          <p class="my-4 text-slate-400">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Enim veniam
            doloremque itaque ad accusantium harum impedit eius modi illo.
            Repellendus.
          </p>
          <div class="flex justify-start items-center gap-3">
            <a
              href="#"
              class="w-12 h-12 bg-white text-black text-2xl rounded-xl flex justify-center items-center"
            >
              <Icon name="lucide:facebook" />
            </a>
            <a
              href="#"
              class="w-12 h-12 bg-white text-black text-2xl rounded-xl flex justify-center items-center"
            >
              <Icon name="lucide:linkedin" />
            </a>
            <a
              href="#"
              class="w-12 h-12 bg-white text-black text-2xl rounded-xl flex justify-center items-center"
            >
              <Icon name="lucide:twitter" />
            </a>
          </div>
        </div>
        <div class="text-slate-400 flex flex-col gap-3">
          <h2 class="font-bold text-2xl text-white">About</h2>
          <a href="#">About Us</a>
          <a href="#">Features</a>
          <a href="#">News & Articles</a>
        </div>
        <div class="text-slate-400 flex flex-col gap-3">
          <h2 class="font-bold text-2xl text-white">Support Us</h2>
          <a href="#">FAQs</a>
          <a href="#">Contact Us</a>
          <a href="#">Support Center</a>
          <a href="#">Security</a>
        </div>
        <div class="text-slate-400 flex flex-col gap-3">
          <h2 class="font-bold text-2xl text-white">Partners</h2>
          <a href="#">Our Partners</a>
          <a href="#">Subscribe</a>
        </div>
      </div>
      <p class="text-white p-5 text-center bg-indigo-900">
        All rights reserved. @tasking.co
      </p>
    </footer>
  </div>
</template>
