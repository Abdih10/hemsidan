<template>
  <nav
    class="top-0 absolute z-50 w-full flex flex-wrap items-center justify-between px-2 py-3 bg-gray-600"
  >
    <div
      class="container px-4 mx-auto flex flex-wrap items-center justify-between"
    >
      <div
        class="w-full relative flex justify-between lg:w-auto lg:static lg:block lg:justify-start"
      >
        <a
          href="#"
          class="flex items- center py-5 px-2 text-white hover:text-gray-500"
        >
          <svg
            class="h-6 w-6 mr-1 text-blue-400"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"
            />
          </svg>
          <span class="font-bold">PSS Skolan?</span> </a
        ><button
          class="cursor-pointer text-xl leading-none px-3 py-1 border-transparent rounded bg-transparent block lg:hidden outline-none focus:outline-none"
          type="button"
          v-on:click="toggleNavbar()"
        >
          <svg
            class="w-8 h-8"
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
      </div>
      <div
        class="lg:flex flex-grow items-center bg-white lg:bg-transparent lg:shadow-none"
        v-bind:class="{ hidden: !showMenu, block: showMenu }"
      >
        <ul class="flex flex-col lg:flex-row list-none lg:ml-auto">
          <li class="flex items-center">
            <router-link
              class="lg:text-white lg:hover:text-gray-300 text-gray-800 px-3 py-4 lg:py-2 flex items-center text-xs font-bold"
              :to="{ name: 'Home' }"
              >Home</router-link
            >
          </li>
          <li class="flex items-center">
            <router-link
              class="lg:text-white lg:hover:text-gray-300 text-gray-800 px-3 py-4 lg:py-2 flex items-center text-xs font-bold"
              :to="{ name: 'Utryckningsrapporter' }"
              >Utryckningsrapporter</router-link
            >
          </li>
          <li class="flex items-center">
            <router-link
              class="lg:text-white lg:hover:text-gray-300 text-gray-800 px-3 py-4 lg:py-2 flex items-center text-xs font-bold"
              :to="{ name: 'Contact' }"
              >Contact</router-link
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
    toggleNavbar: function () {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>
