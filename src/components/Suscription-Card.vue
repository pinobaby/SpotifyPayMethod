<template>
 <header class="bg-black h-20 flex flex-initial items-center justify-start text-white pl-40">
    <img src="../assets/spotifyIcon.png" alt="logo spotify" class=" h-16 w-16">
     <h1>Spotify</h1>
    </header>
    <div class="bg-white py-2 sm:py-2">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="mx-auto max-w-2xl sm:text-center">
            
          <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl pt-4">Elige tu plan Premium</h2>
          
          <p class="mt-6 text-lg leading-8 text-gray-600">Escucha contenido sin límites en tu teléfono, altavoces y otros dispositivos.</p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl rounded-3xl ring-1 ring-gray-200 sm:mt-20 lg:mx-0 lg:flex lg:max-w-none">
          <div class="p-8 sm:p-10 lg:flex-auto">
            <h3 class="text-2xl font-bold tracking-tight text-gray-900">Individual</h3>
            <p class="mt-6 text-base leading-7 text-gray-600">$129.00/mes</p>
            <div class="mt-10 flex items-center gap-x-4">
              <h4 class="flex-none text-sm font-semibold leading-6 text-green-600">Que es lo que incluye?</h4>
              <div class="h-px flex-auto bg-gray-100" />
            </div>
            <div class="mt-10 flex items-start gap-x-4">
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Escucha música sin anuncios</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproduce tus canciones en cualquier lugar, incluso en modo offline</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproduce contenido on-demand</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Elige la opción prepaga o suscríbete</p>
              </div>
            <ul role="list" class="mt-8 grid grid-cols-1 gap-4 text-sm leading-6 text-gray-600 sm:grid-cols-2 sm:gap-6">
              <li v-for="feature in includedFeatures" :key="feature" class="flex gap-x-3">
                {{ feature }}
              </li>
            </ul>
          </div>
          <div class="-mt-2 p-2 lg:mt-0 lg:w-full lg:max-w-md lg:flex-shrink-0">
            <div class="rounded-2xl bg-gray-50 py-10 text-center ring-1 ring-inset ring-gray-900/5 lg:flex lg:flex-col lg:justify-center lg:py-16">
              <div class="mx-auto max-w-xs px-8">
                <p class="text-base font-semibold text-green-500">Un pago único disponible</p>
                <p class="mt-6 flex items-baseline justify-center gap-x-2">
                  <span class="text-5xl font-bold tracking-tight text-gray-900 mb-8">$129.00/mes</span>
                  <span class="text-sm font-semibold leading-6 tracking-wide text-gray-600">MXN</span>
                </p>
           
                  <button 
                  class=" bg-black text-white font-sans rounded-md pl-24 pr-24 pt-2 pb-2 shadow-sm hover:bg-green-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
                  @click="$route.push({name: 'IndidualPlan'})"
                  >
                    Empezar
                  </button>
 
                <!-- <a 
                href="#" 
                class="mt-10 block w-full rounded-md bg-black px-3 py-2 text-center text-sm font-semibold text-white shadow-sm hover:bg-green-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
                @click="$route.path({name: 'SelectIndividual'})"   
                >Empezar</a> -->
                <p class="mt-6 text-xs leading-5 text-gray-600">Se aplican Términos y Condiciones.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-white py-2 sm:py-2">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
    
        <div class="mx-auto mt-3 max-w-2xl rounded-3xl ring-1 ring-gray-200 sm:mt-20 lg:mx-0 lg:flex lg:max-w-none">
          <div class="p-2 sm:p-10 lg:flex-auto">
            <h3 class="text-2xl font-bold tracking-tight text-gray-900">Duo</h3>
            <p class="mt-6 text-base leading-7 text-gray-600">$169.00/mes</p>
            <div class="mt-10 flex items-center gap-x-4">
              <h4 class="flex-none text-sm font-semibold leading-6 text-green-600">Que es lo que incluye?</h4>
              <div class="h-px flex-auto bg-gray-100" />
            </div>
            <div class="mt-10 flex items-start gap-x-4">
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">2 cuentas Premium para dos personas que viven bajo el mismo techo</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproducción de música sin anuncios, en modo offline y on demand</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Elige la opción prepaga o suscríbete</p>
               
              </div>
            <ul role="list" class="mt-8 grid grid-cols-1 gap-4 text-sm leading-6 text-gray-600 sm:grid-cols-2 sm:gap-6">
              <li v-for="feature in includedFeatures" :key="feature" class="flex gap-x-3">
                {{ feature }}
              </li>
            </ul>
          </div>
          <div class="-mt-2 p-2 lg:mt-0 lg:w-full lg:max-w-md lg:flex-shrink-0">
            <div class="rounded-2xl bg-gray-50 py-10 text-center ring-1 ring-inset ring-gray-900/5 lg:flex lg:flex-col lg:justify-center lg:py-16">
              <div class="mx-auto max-w-xs px-8">
                <p class="text-base font-semibold text-green-500">Un pago único disponible</p>
                <p class="mt-6 flex items-baseline justify-center gap-x-2">
                  <span class="text-5xl font-bold tracking-tight text-gray-900 mb-8">$169.00/mes</span>
                  <span class="text-sm font-semibold leading-6 tracking-wide text-gray-600">MXN</span>
                </p>
                <button class=" bg-black text-white font-sans rounded-md pl-24 pr-24 pt-2 pb-2 shadow-sm hover:bg-green-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
                  Empezar
                </button>                
                <p class="mt-6 text-xs leading-5 text-gray-600">Se aplican Términos y Condiciones.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-white py-2 sm:py-2">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
      
        <div class="mx-auto mt-3 max-w-2xl rounded-3xl ring-1 ring-gray-200 sm:mt-20 lg:mx-0 lg:flex lg:max-w-none">
          <div class="p-2 sm:p-10 lg:flex-auto">
            <h3 class="text-2xl font-bold tracking-tight text-gray-900">Para la familia</h3>
            <p class="mt-6 text-base leading-7 text-gray-600">$199.00/mes</p>
            <div class="mt-10 flex items-center gap-x-4">
              <h4 class="flex-none text-sm font-semibold leading-6 text-green-600">Que es lo que incluye?</h4>
              <div class="h-px flex-auto bg-gray-100" />
            </div>
            <div class="mt-10 flex items-start gap-x-4">
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">6 cuentas Premium para familiares que viven bajo el mismo techo</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Bloqueo de música con contenido explícito</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproducción de música sin anuncios, en modo offline y on demand</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Spotify Kids: una aplicación separada hecha solo para niños</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Elige la opción prepaga o suscríbete</p>
                
              </div>
            <ul role="list" class="mt-8 grid grid-cols-1 gap-4 text-sm leading-6 text-gray-600 sm:grid-cols-2 sm:gap-6">
              <li v-for="feature in includedFeatures" :key="feature" class="flex gap-x-3">
                {{ feature }}
              </li>
            </ul>
          </div>
          <div class="-mt-2 p-2 lg:mt-0 lg:w-full lg:max-w-md lg:flex-shrink-0">
            <div class="rounded-2xl bg-gray-50 py-10 text-center ring-1 ring-inset ring-gray-900/5 lg:flex lg:flex-col lg:justify-center lg:py-16">
              <div class="mx-auto max-w-xs px-8">
                <p class="text-base font-semibold text-green-500">Un pago único disponible</p>
                <p class="mt-6 flex items-baseline justify-center gap-x-2">
                  <span class="text-5xl font-bold tracking-tight text-gray-900 mb-8">$199.00/mes</span>
                  <span class="text-sm font-semibold leading-6 tracking-wide text-gray-600">MXN</span>
                </p>
                <button class=" bg-black text-white font-sans rounded-md pl-24 pr-24 pt-2 pb-2 shadow-sm hover:bg-green-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
                  Empezar
                </button>
                <p class="mt-6 text-xs leading-5 text-gray-600">Se aplican Términos y Condiciones.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="bg-white py-2 sm:py-2">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
      
        <div class="mx-auto mt-3 max-w-2xl rounded-3xl ring-1 ring-gray-200 sm:mt-20 lg:mx-0 lg:flex lg:max-w-none">
          <div class="p-2 sm:p-10 lg:flex-auto">
            <h3 class="text-2xl font-bold tracking-tight text-gray-900">Estudiantes</h3>
            <p class="mt-6 text-base leading-7 text-gray-600">$69.00/mes</p>
            <div class="mt-10 flex items-center gap-x-4">
              <h4 class="flex-none text-sm font-semibold leading-6 text-green-600">Que es lo que incluye?</h4>
              <div class="h-px flex-auto bg-gray-100" />
            </div>
            <div class="mt-10 flex items-start gap-x-4">
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Descuento especial para estudiantes universitarios que cumplan con los requisitos</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Escucha música sin anuncios</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproduce tus canciones en cualquier lugar, incluso en modo offline</p>
                <CheckSVG/>
                <p class="text-sm leading-6 text-gray-600">Reproduce contenido on-demand</p>
              </div>
            <ul role="list" class="mt-8 grid grid-cols-1 gap-4 text-sm leading-6 text-gray-600 sm:grid-cols-2 sm:gap-6">
              <li v-for="feature in includedFeatures" :key="feature" class="flex gap-x-3">
                {{ feature }}
              </li>
            </ul>
          </div>
          <div class="-mt-2 p-2 lg:mt-0 lg:w-full lg:max-w-md lg:flex-shrink-0">
            <div class="rounded-2xl bg-gray-50 py-10 text-center ring-1 ring-inset ring-gray-900/5 lg:flex lg:flex-col lg:justify-center lg:py-16">
              <div class="mx-auto max-w-xs px-8">
                <p class="text-base font-semibold text-green-500">Un pago único disponible</p>
                <p class="mt-6 flex items-baseline justify-center gap-x-2">
                  <span class="text-5xl font-bold tracking-tight text-gray-900 mb-8">$69.00/mes</span>
                  <span class="text-sm font-semibold leading-6 tracking-wide text-gray-600">MXN</span>
                </p>
                <button class=" bg-black text-white font-sans rounded-md pl-24 pr-24 pt-2 pb-2 shadow-sm hover:bg-green-600 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600">
                  Empezar
                </button>
                <p class="mt-6 text-xs leading-5 text-gray-600">Se aplican Términos y Condiciones.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
   
  </template>
  
  <script setup>
import CheckSVG from './icons/check-SVG.vue';

  </script>
  