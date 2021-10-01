<template>
  <section class="bg-gray-50">
    <div class="py-16 px-4 overflow-hidden sm:px-6 lg:px-8 lg:py-24">
      <div class="relative max-w-7xl mx-auto">
        <svg
          class="absolute left-full transform translate-x-1/4"
          width="404"
          height="404"
          fill="none"
          viewBox="0 0 404 404"
          aria-hidden="true"
        >
          <defs>
            <pattern
              id="85737c0e-0916-41d7-917f-596dc7edfa27"
              x="0"
              y="0"
              width="20"
              height="20"
              patternUnits="userSpaceOnUse"
            >
              <rect
                x="0"
                y="0"
                width="4"
                height="4"
                class="text-gray-200"
                fill="currentColor"
              />
            </pattern>
          </defs>
          <rect
            width="404"
            height="404"
            fill="url(#85737c0e-0916-41d7-917f-596dc7edfa27)"
          />
        </svg>
        <svg
          class="absolute right-full bottom-0 transform -translate-x-1/4"
          width="404"
          height="404"
          fill="none"
          viewBox="0 0 404 404"
          aria-hidden="true"
        >
          <defs>
            <pattern
              id="85737c0e-0916-41d7-917f-596dc7edfa27"
              x="0"
              y="0"
              width="20"
              height="20"
              patternUnits="userSpaceOnUse"
            >
              <rect
                x="0"
                y="0"
                width="4"
                height="4"
                class="text-gray-200"
                fill="currentColor"
              />
            </pattern>
          </defs>
          <rect
            width="404"
            height="404"
            fill="url(#85737c0e-0916-41d7-917f-596dc7edfa27)"
          />
        </svg>
        <div class="text-center">
          <h2
            class="text-base text-red-600 font-semibold tracking-wide uppercase"
          >
            Contacta con nosotros
          </h2>
          <p
            class="
              mt-2
              text-3xl
              leading-8
              font-extrabold
              tracking-tight
              text-gray-900
              sm:text-4xl
            "
          >
            Dónde estamos
          </p>
          <p class="mt-4 text-lg leading-6 text-gray-500">
            C/ Alcalde Angel Arroyo, 10. Planta 1ª, oficina 1-2.
          </p>
          <p class="mb-4 text-lg leading-6 text-gray-500">
            28904, Getafe, Madrid.
          </p>
        </div>
        <div class="mt-8">
          <TheMap />
        </div>
        <div class="mt-8">
          <div class="max-w-7xl mx-auto">
            <div class="mx-auto md:grid md:grid-cols-2 md:gap-8">
              <div
                class="py-16 px-4 sm:px-6 lg:px-8 bg-white rounded shadow-sm"
              >
                <h2 class="text-2xl font-extrabold text-gray-900 sm:text-3xl">
                  Contacto
                </h2>
                <div class="mt-3">
                  <div class="flex">
                    <div class="flex-shrink-0">
                      <svg
                        class="h-6 w-6 text-gray-400"
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
                          d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"
                        />
                      </svg>
                    </div>
                    <div class="ml-3 text-lg text-gray-500">
                      <p>
                        <a href="tel:91 330 49 96">91 330 49 96</a>
                      </p>
                    </div>
                  </div>
                  <div class="mt-3 flex">
                    <div class="flex-shrink-0">
                      <svg
                        class="h-6 w-6 text-gray-400"
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
                          d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
                        />
                      </svg>
                    </div>
                    <div class="ml-3 text-lg text-gray-500">
                      <p class="break-all">administracion@eliteasesor.com</p>
                    </div>
                  </div>
                </div>
              </div>
              <div
                class="
                  py-16
                  px-4
                  sm:px-6
                  lg:px-8
                  mt-8
                  md:mt-0
                  bg-white
                  rounded
                  shadow-sm
                "
              >
                <h2 class="text-2xl font-extrabold text-gray-900 sm:text-3xl">
                  Horario
                </h2>
                <div class="mt-3">
                  <p class="text-lg text-gray-500">
                    Lunes a jueves de 09:00h a 14:00h y de 15:30h a 19:00h.
                  </p>
                  <p class="text-lg text-gray-500">
                    Viernes de 09:00h a 15:00h.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import TheMap from '~/components/TheMap'

export default {
  name: 'MoreServicesSection',
  components: { TheMap },
}
</script>
