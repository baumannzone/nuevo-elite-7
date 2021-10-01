<template>
  <!-- This example requires Tailwind CSS v2.0+ -->
  <nav class="bg-gray-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex items-center">
          <div class="flex-shrink-0">
            <img
              class="block h-8 w-auto"
              src="/elite7-blanco.png"
              alt="Elite 7 Asesor"
              width="107"
              height="32"
            />
          </div>
          <div class="hidden sm:block sm:ml-6">
            <div class="flex space-x-4">
              <NuxtLink
                v-for="item in navItems"
                :key="item.displayText"
                :to="item.to"
                class="
                  text-white
                  px-3
                  py-2
                  rounded-md
                  text-sm
                  font-medium
                  hover:bg-gray-700 hover:text-white
                "
              >
                {{ item.displayText }}
              </NuxtLink>
            </div>
          </div>
        </div>
        <div class="-mr-2 flex sm:hidden">
          <button
            class="
              inline-flex
              items-center
              justify-center
              p-2
              rounded-md
              text-gray-400
              bg-gray-700
              hover:text-white hover:bg-gray-500
              focus:outline-none focus:ring-2 focus:ring-insest focus:ring-white
            "
            aria-expanded="false"
            @click="showMenu = !showMenu"
          >
            <span class="sr-only">Open main menu</span>
            <svg
              :class="showMenu ? 'hidden' : 'block'"
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
            <svg
              :class="showMenu ? 'block' : 'hidden'"
              class="h-6 w-6"
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              aria-hidden="true"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>
    <div v-show="showMenu" class="block sm:hidden">
      <div class="px-2 pt-2 pb-3 space-y-1">
        <NuxtLink
          v-for="item in navItems"
          :key="item.displayText"
          :to="item.to"
          class="
            block
            text-white
            px-3
            py-2
            rounded-md
            text-sm
            font-medium
            hover:bg-gray-700 hover:text-white
          "
        >
          {{ item.displayText }}
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>

<script>
const navItems = [
  { displayText: 'Inicio', to: '/' },
  { displayText: 'Servicios', to: '/servicios' },
  { displayText: 'Contacto', to: '/contacto' },
]
export default {
  name: 'NavigationBar',
  data() {
    return {
      navItems,
      showMenu: false,
    }
  },
  watch: {
    $route() {
      this.showMenu = false
    },
  },
}
</script>

<style>
.nuxt-link-exact-active {
  @apply bg-gray-500 text-white;
}
</style>
