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
  </div>
</template>
