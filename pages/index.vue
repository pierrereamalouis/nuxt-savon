<template>
  <section
    class="relative bg-cover bg-center bg-no-repeat min-h-[720px] flex items-center"
    style="background-image: url('/img/naturally-pure-soaps-hero.png')"
  >
    <div class="container mx-auto px-6 md:px-12 lg:px-20">
      <div class="max-w-2xl text-left">
        <h1 class="text-4xl md:text-5xl font-semibold leading-tight text-gray-900">
          Naturellement
          <span class="text-orange-600"> Purs, </span>
          <br />
          <span class="text-green-700"> Soigneus</span>ement Façonnés
        </h1>

        <p class="mt-4 text-lg text-gray-700">
          Découvrez notre collection de savons bio faits main — Offrez à votre peau ce que la nature
          a de meilleur.
        </p>

        <div class="mt-6">
          <NuxtLink
            to="/boutique"
            class="inline-block bg-purple-100 text-purple-700 border border-purple-400 hover:bg-purple-200 hover:text-purple-900 transition font-medium py-2 px-6 rounded-full"
          >
            Découvrir la boutique
          </NuxtLink>
        </div>
      </div>
    </div>
  </section>

  <section class="py-12 bg-gray-100">
    <div class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
      <div class="p-6 bg-white rounded-md shadow-md">
        <div
          class="w-16 h-16 mx-auto bg-green-200 text-green-600 rounded-full flex items-center justify-center mb-4"
        >
          <svg
            class="w-8 h-8"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"
            ></path>
          </svg>
        </div>
        <h3 class="text-xl font-semibold text-gray-700 mb-2">Ingrédients Naturels</h3>
        <p class="text-gray-500">Des ingrédients purs pour une peau saine.</p>
      </div>
      <div class="p-6 bg-white rounded-md shadow-md">
        <div
          class="w-16 h-16 mx-auto bg-blue-200 text-blue-600 rounded-full flex items-center justify-center mb-4"
        >
          <svg
            class="w-8 h-8"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M17 13l-5 5m0-5l5 5m2-2l-5-5m5 5l-5-5"
            ></path>
          </svg>
        </div>
        <h3 class="text-xl font-semibold text-gray-700 mb-2">Fabrication Artisanale</h3>
        <p class="text-gray-500">Savons faits à la main avec soin.</p>
      </div>
      <div class="p-6 bg-white rounded-md shadow-md">
        <div
          class="w-16 h-16 mx-auto bg-yellow-200 text-yellow-600 rounded-full flex items-center justify-center mb-4"
        >
          <svg
            class="w-8 h-8"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M15 5l-1.5 1.5M19 11l-6 6m-2-2L15 7M3 13l4-4m0 0L19 7m-6 6l-4-4m4 4L3 13"
            ></path>
          </svg>
        </div>
        <h3 class="text-xl font-semibold text-gray-700 mb-2">Respectueux de la Peau</h3>
        <p class="text-gray-500">Formules douces pour tous les types de peau.</p>
      </div>
    </div>
  </section>

  <section class="py-16 bg-white">
    <div class="container mx-auto">
      <h2 class="text-2xl font-semibold text-gray-800 mb-8 text-center">
        Découvrez Notre Collection
      </h2>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/products/savon-1">
            <img src="/img/soap-1.jpg" alt="Savon 1" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Douceur</h3>
              <p class="text-gray-500 text-sm">Un savon doux pour une utilisation quotidienne.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/products/savon-2">
            <img src="/img/soap-2.jpg" alt="Savon 2" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Exfoliant</h3>
              <p class="text-gray-500 text-sm">Pour une peau lisse et renouvelée.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/products/savon-3">
            <img src="/img/soap-3.jpg" alt="Savon 3" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Parfumé</h3>
              <p class="text-gray-500 text-sm">Un parfum délicat pour une sensation agréable.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/products/savon-4">
            <img src="/img/soap-4.jpg" alt="Savon 4" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Hydratant</h3>
              <p class="text-gray-500 text-sm">Pour une peau douce et hydratée.</p>
            </div>
          </NuxtLink>
        </div>
      </div>
      <div class="text-center mt-8">
        <NuxtLink
          to="/products"
          class="inline-block bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-6 rounded-full"
          >Voir Toute la Collection</NuxtLink
        >
      </div>
    </div>
  </section>

  <section class="py-12 bg-gray-50">
    <div class="container mx-auto text-center">
      <h2 class="text-2xl font-semibold text-gray-800 mb-6">Explorez Nos Catégories</h2>
      <div class="space-x-4">
        <NuxtLink
          to="/products?category=exfoliant"
          class="inline-block bg-white hover:bg-gray-200 text-gray-700 font-semibold py-2 px-4 rounded-full shadow-sm"
          >Savons Exfoliants</NuxtLink
        >
        <NuxtLink
          to="/products?category=hydratant"
          class="inline-block bg-white hover:bg-gray-200 text-gray-700 font-semibold py-2 px-4 rounded-full shadow-sm"
          >Savons Hydratants</NuxtLink
        >
        <NuxtLink
          to="/products?category=parfume"
          class="inline-block bg-white hover:bg-gray-200 text-gray-700 font-semibold py-2 px-4 rounded-full shadow-sm"
          >Savons Parfumés</NuxtLink
        >
        <NuxtLink
          to="/products?category=doux"
          class="inline-block bg-white hover:bg-gray-200 text-gray-700 font-semibold py-2 px-4 rounded-full shadow-sm"
          >Savons Doux</NuxtLink
        >
      </div>
    </div>
  </section>
</template>

<script setup lang="ts"></script>

<style scoped></style>
