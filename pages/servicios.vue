<template>
  <div>
    <div class="bg-red-50">
      <div class="container">
        <div
          class="
            max-w-7xl
            mx-auto
            py-12
            px-4
            sm:px-6
            lg:py-24 lg:px-8 lg:flex lg:items-center lg:justify-between
          "
        >
          <h2
            class="
              text-3xl
              font-extrabold
              tracking-tight
              text-gray-900
              md:text-4xl
            "
          >
            <span class="block">Consultores y asesores.</span>
            <span class="block text-red-600">Estamos aquí para ayudarte.</span>
          </h2>

          <div class="mt-8 flex lg:mt-0 lg:flex-shrink-0">
            <div class="flex rounded-md shadow">
              <nuxt-link
                to="contacto"
                target="_blank"
                class="
                  inline-flex
                  items-center
                  justify-center
                  px-5
                  py-3
                  border border-transparent
                  text-base
                  font-bold
                  rounded-md
                  text-white
                  bg-red-600
                  hover:bg-red-700
                "
              >
                Quiero asesoramiento
              </nuxt-link>
            </div>
          </div>
        </div>
      </div>
    </div>

    <section>
      <div class="py-16 bg-gray-50 overflow-hidden lg:py-24">
        <div
          class="relative max-w-xl mx-auto px-4 sm:px-6 lg:px-8 lg:max-w-7xl"
        >
          <svg
            class="
              hidden
              lg:block
              absolute
              left-full
              transform
              -translate-x-1/2 -translate-y-1/4
            "
            width="404"
            height="684"
            fill="none"
            viewBox="0 0 404 784"
            aria-hidden="true"
          >
            <defs>
              <pattern
                id="b1e6e422-73f8-40a6-b5d9-c8586e37e0e7"
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
              height="784"
              fill="url(#b1e6e422-73f8-40a6-b5d9-c8586e37e0e7)"
            />
          </svg>

          <!-- Header -->
          <div class="relative">
            <h2
              class="
                text-center text-3xl
                leading-8
                font-extrabold
                tracking-tight
                text-gray-900
                sm:text-4xl
              "
            >
              Haz crecer tu negocio
            </h2>
            <p class="mt-4 max-w-3xl mx-auto text-center text-xl text-gray-500">
              Consultoría y asesoría de élite. Ahorra tiempo en la gestión de tu
              negocio. Evita errores y sanciones de Hacienda.
            </p>
          </div>

          <!-- Main title -->
          <div class="relative mt-12 lg:mt-24 lg:items-center">
            <div class="relative">
              <h3
                class="
                  text-2xl
                  font-extrabold
                  text-gray-900
                  tracking-tight
                  sm:text-3xl
                "
              >
                Asesores y consultores
              </h3>
              <p class="mt-3 text-lg text-gray-500">
                Te asesoramos y acompañamos en lo que necesites para hacer
                crecer tu negocio.
              </p>

              <dl class="mt-10 space-y-10">
                <!-- Block 1 -->
                <div class="relative">
                  <dt>
                    <div
                      class="
                        absolute
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
                      <svg-fiscal></svg-fiscal>
                    </div>
                    <p class="ml-16 text-xl leading-6 font-bold text-gray-900">
                      Asesoramiento Fiscal
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Asesoramiento e información fiscal actualizada al cliente en
                    su actividad empresarial.
                    <ItemsList :items="fiscalItems" />
                  </dd>
                </div>

                <!-- Block 2 -->
                <div class="relative">
                  <dt>
                    <div
                      class="
                        absolute
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
                      <svg-contable></svg-contable>
                    </div>
                    <p class="ml-16 text-xl leading-6 font-bold text-gray-900">
                      Asesoramiento Contable
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Asesoramiento contable y confección de contabilidades a
                    entidades mercantiles y autónomos.

                    <ItemsList :items="contableItems" />
                  </dd>
                </div>
              </dl>
            </div>

            <div class="mt-10 -mx-4 relative lg:mt-0" aria-hidden="true">
              <svg
                class="
                  absolute
                  left-1/2
                  transform
                  -translate-x-1/2
                  translate-y-16
                  lg:hidden
                "
                width="684"
                height="404"
                fill="none"
                viewBox="0 0 784 404"
              >
                <defs>
                  <pattern
                    id="ca9667ae-9f92-4be7-abcb-9e3d727f2941"
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
                  width="784"
                  height="404"
                  fill="url(#ca9667ae-9f92-4be7-abcb-9e3d727f2941)"
                />
              </svg>
              <img
                class="relative mx-auto mt-10"
                width="490"
                src="/servicios/spreadsheet.svg"
                alt="ilustración hoja de excel"
              />
            </div>
          </div>

          <svg
            class="hidden lg:block absolute right-full transform translate-y-12"
            width="404"
            height="784"
            fill="none"
            viewBox="0 0 404 784"
            aria-hidden="true"
          >
            <defs>
              <pattern
                id="64e643ad-2176-4f86-b3d7-f2c5da3b6a6d"
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
              height="784"
              fill="url(#64e643ad-2176-4f86-b3d7-f2c5da3b6a6d)"
            />
          </svg>

          <div class="relative mt-12 sm:mt-16 lg:mt-24">
            <div class="lg:items-center">
              <div class="lg:col-start-2">
                <!-- <h3
                  class="text-2xl font-extrabold text-gray-900 tracking-tight sm:text-3xl"
                >
                  Particulares o Empresas
                </h3>
                <p class="mt-3 text-lg text-gray-500">
                  Resolvemos sus problemas, minimizamos sus riesgos y le
                  ahorramos tiempo y recursos. ¡Llama ya!
                </p> -->

                <dl class="mt-10 space-y-10">
                  <!-- Block 3 -->
                  <div class="relative">
                    <dt>
                      <div
                        class="
                          absolute
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
                        <svg-juridico></svg-juridico>
                      </div>
                      <p
                        class="ml-16 text-xl leading-6 font-bold text-gray-900"
                      >
                        Asesoramiento Jurídico
                      </p>
                    </dt>
                    <dd class="mt-2 ml-16 text-base text-gray-500">
                      Disponemos de profesionales que prestan sus servicios en
                      todas las ramas del derecho:

                      <ItemsList :items="juridicoItems" />
                    </dd>
                  </div>

                  <!-- Block 4 -->
                  <div class="relative">
                    <dt>
                      <div
                        class="
                          absolute
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
                        <svg-laboral></svg-laboral>
                      </div>
                      <p
                        class="ml-16 text-xl leading-6 font-bold text-gray-900"
                      >
                        Asesoramiento Laboral
                      </p>
                    </dt>
                    <dd class="mt-2 ml-16 text-base text-gray-500">
                      Elaboración de nóminas, seguros sociales, impuestos.
                      Altas, bajas, modificaciones en Seguridad Social.

                      <ItemsList :items="laboralItems" />
                    </dd>
                  </div>
                </dl>
              </div>

              <div class="mt-10 -mx-4 relative lg:mt-0 lg:col-start-1">
                <svg
                  class="absolute left-1/2 transform translate-y-16 lg:hidden"
                  width="784"
                  height="404"
                  fill="none"
                  viewBox="0 0 784 404"
                  aria-hidden="true"
                >
                  <defs>
                    <pattern
                      id="e80155a9-dfde-425a-b5ea-1f6fadd20131"
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
                    width="784"
                    height="404"
                    fill="url(#e80155a9-dfde-425a-b5ea-1f6fadd20131)"
                  />
                </svg>
                <img
                  class="relative mx-auto mt-10"
                  width="490"
                  src="/servicios/agreement.svg"
                  alt="ilustración contrato"
                />
              </div>
            </div>
          </div>

          <!-- extra block -->
          <div class="relative mt-12 lg:mt-24 lg:items-center">
            <div class="relative">
              <dl class="mt-10 space-y-10">
                <!-- Block 1 -->
                <div class="relative">
                  <dt>
                    <div
                      class="
                        absolute
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
                      <svg-otros></svg-otros>
                    </div>
                    <p class="ml-16 text-xl leading-6 font-bold text-gray-900">
                      Otros servicios
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Además, ofrecemos otros servicios como:
                    <ItemsList :items="otrosItems" />
                  </dd>
                </div>

                <!-- Block 2 -->
                <div class="relative">
                  <dt>
                    <div
                      class="
                        absolute
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
                      <svg-colaboradores></svg-colaboradores>
                    </div>
                    <p class="ml-16 text-xl leading-6 font-bold text-gray-900">
                      Colaboradores
                    </p>
                  </dt>
                  <dd class="mt-2 ml-16 text-base text-gray-500">
                    Contamos con colaboradores externos expertos en otras áreas
                    necesarias para el desarrollo de cualquier actividad
                    empresarial o profesional.

                    <ItemsList :items="colaboradoresItems" />
                  </dd>
                </div>
              </dl>
            </div>

            <div class="mt-10 -mx-4 relative lg:mt-0" aria-hidden="true">
              <svg
                class="
                  absolute
                  left-1/2
                  transform
                  -translate-x-1/2
                  translate-y-16
                  lg:hidden
                "
                width="684"
                height="404"
                fill="none"
                viewBox="0 0 784 404"
              >
                <defs>
                  <pattern
                    id="ca9667ae-9f92-4be7-abcb-9e3d727f2941"
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
                  width="784"
                  height="404"
                  fill="url(#ca9667ae-9f92-4be7-abcb-9e3d727f2941)"
                />
              </svg>
              <img
                class="relative mx-auto mt-10"
                width="490"
                src="/servicios/files.svg"
                alt="ilustración hoja de excel"
              />
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ItemsList from '@/components/servicios/ItemsList.vue'
import {
  SvgLaboral,
  SvgContable,
  SvgJuridico,
  SvgFiscal,
  SvgOtros,
  SvgColaboradores,
} from '~/components/svgIcons/index.js'

export default {
  name: 'Servicios',
  components: {
    SvgLaboral,
    SvgContable,
    SvgJuridico,
    SvgFiscal,
    SvgOtros,
    SvgColaboradores,
    ItemsList,
  },
  data() {
    return {
      fiscalItems: [
        'Planificación fiscal.',
        'Preparación y presentación de los impuestos relativos a la actividad de la	empresa.',
        'Impuesto sobre el valor añadido (IVA).	',
        'Retenciones y pagos a cuenta de IRPF, sociedades y arrendamientos.',
        'Pagos a cuenta de empresarios individuales o profesionales.',
        'Impuestos de Sociedades.',
        'Impuestos sobre la Renta de las Personas Físicas.',
        'Representación y asistencia ante la Agencia Tributaria en Inspecciones Fiscales.',
        'Atención de requerimientos de la Agencia Tributaria.',
      ],
      contableItems: [
        'Supervisión y revisión de la contabilidad adaptada al PGC.',
        'Elaboración y presentación de los libros oficiales.',
        'Elaboración y presentación de las cuentas anuales.',
        'Información actualizada de la normativa contable.',
        'Actualización de contabilidades atrasadas.',
      ],
      juridicoItems: [
        ' Civil',
        ' Familiar',
        ' Penal',
        ' Administrativo',
        ' Tributario',
        ' Mercantil',
      ],
      laboralItems: [
        'Altas, bajas y modificaciones de trabajadores en Seguridad Social.',
        'Elaboración, tramitación y contratos de trabajo.',
        'Elaboración de nóminas mensuales.',
        'Confección de boletines de cotización a la Seguridad Social.',
        'Modelo 111 de retenciones y modelo 190 resumen anual.',
        'Confección de certificados de tribuciones y retenciones de los trabajadores.',
        'Asesoramiento en las dudas y problemas de carácter laboral que se presenten.',
        'Asistencia en Inspecciones de Trabajo y Seguridad Social.',
        'Asistencia ante el servicio de mediación, arbitraje y conciliación.',
        'Redacción y tramitación de recusos por sanciones.',
        'Alta en regímenes especiales.',
        'Solicitud de prestaciones (maternidad, paternidad, jubilación, viudedad, orfandad, etc.)	',
        'Tramitación de expedientes de regulación de empleo.',
        'Defensa ante los Juzgados de lo social por despidos, sanciones y reclamaciones.',
      ],
      otrosItems: [
        'Elaboración y presentación de INTRASTAT.',
        'Información y tramitación de subvenciones.',
        'Licencias de apertura de actividades.',
        'Impuestos especiales.',
      ],
      colaboradoresItems: [
        'Auditoria de cuentas.',
        'Adecuación a la LOPD.',
        'Servicio de prevención de riesgos laborales.',
        'Servicio de protección de datos.',
      ],
    }
  },
}
</script>
