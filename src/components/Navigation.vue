<template>
  <!-- navbar goes here -->
  <nav class="bg-gray-200">
    <div class="max-w-8xl mx-auto px-4">
      <!-- Kolla med gruppen om hur långt ifrån varandra länkerna ska vara. Antigen between eller around som det är just nu. -->
      <div class="flex justify-around">
        <div class="flex space-x-4">
          <!-- logo -->
          <div>
            <a
              href="#"
              class="flex items- center py-5 px-2 text-gray-700 hover:text-gray-900"
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
              <span class="font-bold">PSS Skolan?</span>
            </a>
          </div>
        </div>

        <!-- nav -->
        <div class="hidden md:flex items-center space-x-1">
          <router-link
            class="block py-2 px-4 text-sm hover:bg-gray-200"
            :to="{ name: 'Home' }"
            >Home</router-link
          >
          <router-link
            class="block py-2 px-4 text-sm hover:bg-gray-200"
            :to="{ name: 'Utryckningsrapporter' }"
            >Utryckningsrapporter</router-link
          >
          <router-link
            class="block py-2 px-4 text-sm hover:bg-gray-200"
            :to="{ name: 'Contact' }"
            >Contact</router-link
          >
          <button
            class="text-white bg-blue-500 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-3 py-1 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
            type="button"
            style="transition: all 0.15s ease 0s"
          >
            <router-link
              class="lg:text-blue lg:hover:text-gray-300 text-gray-800 px-3 py-4 lg:py-2 flex items-center text-s font-bold"
              :to="{ name: 'Login' }"
              >Login</router-link
            >
          </button>
        </div>

        <!-- mobile button goes here -->
        <div class="md:hidden flex items-center">
          <button class="mobile-menu-button" v-on:click="toggleNavbar()">
            <svg
              class="w-6 h-6"
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
      </div>
    </div>

    <!-- mobile menu -->
    <div class="mobile-menu hidden md:hidden">
      <router-link
        class="block py-2 px-4 text-sm hover:bg-gray-200"
        :to="{ name: 'Home' }"
        >Home</router-link
      >
      <router-link
        class="block py-2 px-4 text-sm hover:bg-gray-200"
        :to="{ name: 'Utryckningsrapporter' }"
        >Utryckningsrapporter</router-link
      >
      <router-link
        class="block py-2 px-4 text-sm hover:bg-gray-200"
        :to="{ name: 'Contact' }"
        >Contact</router-link
      >
      <button
        class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
        type="button"
        style="transition: all 0.15s ease 0s"
      >
        <router-link
          class="lg:text-white lg:hover:text-gray-300 text-gray-800 px-3 py-4 lg:py-2 flex items-center text-s font-bold"
          :to="{ name: 'Login' }"
          >Login</router-link
        >
      </button>
    </div>
  </nav>
</template>
<script>
export default {
  name: "Navigation",
  // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    // eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
    toggleNavbar: function () {
      const btn = document.querySelector(".mobile-menu-button");
      const menu = document.querySelector(".mobile-menu");
      btn.addEventListener("click", () => {
        menu.classList.toggle("hidden");
      });
    },
  },
};
</script>
