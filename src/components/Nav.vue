<template>
  <nav class="border-gray-200 px-2 sm:px-4 py-2.5">
    <div class="flex flex-wrap items-center justify-between mx-auto">
      <router-link to="/" class="font-bold text-3xl text-gray-100 hidden w-full md:block md:w-auto transition duration-700 ease-in-out hover:scale-110">DT</router-link>
      <!-- <button data-collapse-toggle="navbar-default" type="button"
        class="inline-flex items-center p-2 ml-3 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600"
        aria-controls="navbar-default" aria-expanded="false" @click="swichMenu">
        <span class="sr-only">Open main menu</span>
        <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20"
          xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd"
            d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
            clip-rule="evenodd"></path>
        </svg>
      </button> -->
      <div class="w-full md:w-auto" id="navbar-default">
        <ul
          class="flex justify-center mt-4 border border-gray-100 rounded-lg md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0  dark:border-gray-700 ">
          <router-link to="/" class="block py-2 pl-3 pr-4 text-white rounded md:bg-transparent md:p-0 transition duration-700 ease-in-out hover:scale-110  hover:underline">
            MAIN
          </router-link>
          <router-link to="/about"
            class="block py-2 pl-3 pr-4 text-white hover:text-green-500 rounded md:bg-transparent md:p-0 transition duration-700 ease-in-out hover:scale-110 hover:underline">
            <span class="">
              ABOUT
            </span>
          </router-link>
          <img src="https://flowbite.com/docs/images/logo.svg" class="h-6 mx-6 sm:h-6" />

          <router-link to="/skills"
            class="block py-2 pl-3 pr-4 text-white rounded md:bg-transparent md:p-0 transition duration-700 ease-in-out hover:scale-110 hover:underline">
            SKILLS
          </router-link>
          <router-link to="/contact"
            class="block py-2 pl-3 pr-4 text-white rounded md:bg-transparent md:p-0 transition duration-700 ease-in-out hover:scale-110 hover:underline">
            CONTACT
          </router-link>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import { ref } from 'vue'
// import { RouterLink } from 'vue-router'

export default {
  setup() {
    const daniel = ref('Daniel')
    const openMenu = ref(false)

    const swichMenu = () => openMenu.value = !openMenu.value

    return { daniel, openMenu, swichMenu }
  }
}
</script>

<style></style>