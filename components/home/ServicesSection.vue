<template>
  <div class="container">
    <section>
      <!-- This example requires Tailwind CSS v2.0+ -->
      <div class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div class="text-center">
            <h2
              class="
                text-base text-red-600
                font-semibold
                tracking-wide
                uppercase
              "
            >
              Nuestros servicios
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
              Consultoría y asesoramiento
            </p>
            <p class="mt-4 max-w-2xl text-xl text-gray-500 lg:mx-auto">
              Prestamos servicios de consultoría y asesoramiento fiscal,
              contable, jurídico y laboral. Para ti o para tu empresa.
            </p>
          </div>

          <div class="mt-14">
            <div
              class="
                space-y-10
                md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10
              "
            >
              <div class="flex">
                <div class="flex-shrink-0">
                  <div
                    class="
                      flex
                      items-center
                      justify-center
                      h-12
                      w-12
                      rounded-md
                      bg-red-500
                      text-white
                    "
                  >
                    <SvgFiscal></SvgFiscal>
                  </div>
                </div>
                <div class="ml-4">
                  <dl>
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Fiscal
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento en todo tipo de materia tributaria a
                      empresas, autónomos y particulares.
                    </dd>
                  </dl>
                </div>
              </div>

              <div class="flex">
                <div class="flex-shrink-0">
                  <div
                    class="
                      flex
                      items-center
                      justify-center
                      h-12
                      w-12
                      rounded-md
                      bg-red-500
                      text-white
                    "
                  >
                    <SvgContable></SvgContable>
                  </div>
                </div>
                <div class="ml-4">
                  <dl>
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Contable
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento contable y confección de contabilidades a
                      entidades mercantiles y autónomos.
                    </dd>
                  </dl>
                </div>
              </div>

              <div class="flex">
                <div class="flex-shrink-0">
                  <div
                    class="
                      flex
                      items-center
                      justify-center
                      h-12
                      w-12
                      rounded-md
                      bg-red-500
                      text-white
                    "
                  >
                    <SvgJuridico></SvgJuridico>
                  </div>
                </div>
                <div class="ml-4">
                  <dl>
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Jurídico
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Asesoramiento en derecho mercantil, tributario y laboral.
                      Derecho civil, penal y administrativo.
                    </dd>
                  </dl>
                </div>
              </div>

              <div class="flex">
                <div class="flex-shrink-0">
                  <div
                    class="
                      flex
                      items-center
                      justify-center
                      h-12
                      w-12
                      rounded-md
                      bg-red-500
                      text-white
                    "
                  >
                    <SvgLaboral></SvgLaboral>
                  </div>
                </div>
                <div class="ml-4">
                  <dl>
                    <dt class="text-lg leading-6 font-medium text-gray-900">
                      Asesoramiento Laboral
                    </dt>
                    <dd class="mt-2 text-base text-gray-500">
                      Todo tipo de asesoramiento laboral.
                    </dd>
                  </dl>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import {
  SvgLaboral,
  SvgContable,
  SvgJuridico,
  SvgFiscal,
} from '~/components/svgIcons/index.js'

export default {
  name: 'ServicesSection',
  components: { SvgLaboral, SvgContable, SvgJuridico, SvgFiscal },
}
</script>
