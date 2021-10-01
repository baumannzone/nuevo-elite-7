<template>
  <footer class="bg-gray-800">
    <div class="max-w-7xl mx-auto py-20 px-4 overflow-hidden sm:px-6 lg:px-8">
      <nav
        class="-mx-5 -my-2 flex flex-wrap justify-center"
        aria-label="Footer"
      >
        <div v-for="item in navItems" :key="item.to" class="px-5 py-2">
          <a
            :href="item.to"
            class="text-base text-gray-300 hover:text-gray-500"
          >
            {{ item.text }}
          </a>
        </div>
      </nav>

      <p class="mt-8 text-center text-base text-gray-400">
        Todos los derechos reservados · &copy; 2021 Consultores y Asesores Élite
        7, S.L.
      </p>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'TheFooter',
  data() {
    return {
      navItems: [
        {
          text: 'Inicio',
          to: '/',
        },
        {
          text: 'Servicios',
          to: '/servicios',
        },
        {
          text: 'Contacto',
          to: '/contacto',
        },
      ],
    }
  },
}
</script>
