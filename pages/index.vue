<template>
  <section class="w-[100%] relative h-[75vh] flex items-center">
    <img
      src="/img/naturally-pure-soaps-cover.png"
      alt="les mains moussantes"
      class="w-[100%] h-[75vh] object-cover"
    />
    <div class="absolute mx-auto px-6 md:px-12 lg:px-20">
      <div class="max-w-2xl text-left">
        <h1 class="font-handwritten text-5xl md:text-6xl font-semibold leading-tight text-gray-900">
          Naturellement
          <span class="font-handwritten text-orange-600"> Purs, </span>
          <br />
          <span class="font-handwritten text-green-700"> Soigneus</span>ement Façonnés
        </h1>

        <p class="font-sans mt-4 text-lg text-gray-700">
          Découvrez notre collection de savons bio faits main — Offrez à votre peau ce que la nature
          a de meilleur.
        </p>

        <div class="mt-6">
          <NuxtLink
            to="/boutique"
            class="font-sans bg-gray-200 text-gray-800 border border-gray-300 hover:bg-gray-200 hover:text-black transition font-medium py-2 px-6 rounded-full"
          >
            Découvrir la boutique
          </NuxtLink>
        </div>
      </div>
    </div>
  </section>

  <section class="bg-white py-12">
    <div class="container mx-auto px-6 lg:px-20">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10 text-center">
        <!-- Item 1 -->
        <div class="flex flex-col items-center">
          <img src="/icons/delivery.png" alt="Livraison Rapide" class="h-10 mb-3" />
          <h3 class="text-lg font-semibold text-gray-800">Livraison Rapide</h3>
          <p class="text-sm text-gray-600">Expédition éclair</p>
        </div>

        <!-- Item 2 -->
        <div class="flex flex-col items-center">
          <img src="/icons/payment.png" alt="Paiement Sécurisé" class="h-10 mb-3" />
          <h3 class="text-lg font-semibold text-gray-800">Paiement Sécurisé</h3>
          <p class="text-sm text-gray-600">Achetez en toute confiance</p>
        </div>

        <!-- Item 3 -->
        <div class="flex flex-col items-center">
          <img src="/icons/refund.png" alt="Satisfait ou Remboursé" class="h-10 mb-3" />
          <h3 class="text-lg font-semibold text-gray-800">Satisfait ou Remboursé</h3>
          <p class="text-sm text-gray-600">Garantie 100% remboursé</p>
        </div>

        <!-- Item 4 -->
        <div class="flex flex-col items-center">
          <img src="/icons/support.png" alt="Assistance 24h/7j" class="h-10 mb-3" />
          <h3 class="text-lg font-semibold text-gray-800">Assistance 24h/7j</h3>
          <p class="text-sm text-gray-600">Toujours là pour vous</p>
        </div>
      </div>
    </div>
  </section>

  <section class="bg-gray-100 py-16 px-6 md:px-12">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl md:text-4xl font-bold text-center mb-12">Prix & Promotion</h2>

      <div class="grid md:grid-cols-2 gap-12 items-center">
        <!-- Top Text & Image -->
        <div class="flex flex-col gap-6">
          <div class="flex items-center gap-3">
            <span class="text-xl">✨</span>
            <p class="text-lg text-gray-800">
              Notre produit est offert à <span class="font-semibold">$8.50</span> pour 100 grammes
            </p>
          </div>

          <div class="flex items-center gap-3">
            <p class="text-lg text-gray-800">10% de rabais lors de votre commande en ligne</p>
            <span class="text-xl">✨</span>
          </div>

          <div class="flex items-center gap-3">
            <span class="text-xl">✨</span>
            <p class="text-lg text-gray-800">
              Recevez 1 barre gratuite à l’achat de 8 barres<span class="text-sm text-gray-500"
                >*</span
              >
            </p>
          </div>

          <p class="text-sm text-gray-500 mt-4">*Pour les membres du programme de fidélité</p>
        </div>

        <!-- Images (stacked on mobile) -->
        <div class="grid grid-cols-2 gap-4">
          <img
            src="/img/soap-promo-1.jpg"
            alt="Savon 1"
            class="rounded-lg shadow-md object-cover h-64 w-full"
          />
          <img
            src="/img/soap-promo-2.jpg"
            alt="Savon 2"
            class="rounded-lg shadow-md object-cover h-64 w-full"
          />
        </div>
      </div>
    </div>
  </section>

  <section class="bg-white py-16 px-6 md:px-12">
    <div class="max-w-7xl mx-auto">
      <div class="grid md:grid-cols-3 gap-6">
        <!-- Card 1 -->
        <div class="relative bg-green-100 p-6 rounded-lg shadow-md overflow-hidden">
          <h3 class="text-xl font-semibold mb-4">100% Ingrédients Naturels</h3>
          <ul class="text-sm text-gray-700 space-y-1 mb-4">
            <li>Huile de coco</li>
            <li>Glycérine</li>
            <li>Vitamine E</li>
            <li>Miel</li>
          </ul>
          <NuxtLink to="/produit" class="text-sm font-medium text-gray-800 hover:underline">
            Voir la boutique
          </NuxtLink>
          <!-- Product Image -->
          <img
            src="/img/ingredients_naturel.png"
            alt="Savon Naturel"
            class="absolute right-2 bottom-2 w-28 h-auto object-contain z-10"
          />
        </div>

        <!-- Card 2 -->
        <div class="relative bg-rose-50 p-6 rounded-lg shadow-md overflow-hidden">
          <h3 class="text-xl font-semibold mb-4">Sans cruauté & Écoresponsable</h3>
          <p class="text-sm text-gray-700 mb-4">
            Des produits respectueux de votre peau et de la planète.
          </p>
          <NuxtLink to="/produit" class="text-sm font-medium text-gray-800 hover:underline">
            Voir la boutique
          </NuxtLink>
          <img
            src="/img/ecoresponsable.png"
            alt="Feuilles naturelles"
            class="absolute right-2 bottom-2 w-28 h-auto object-contain z-10"
          />
        </div>

        <!-- Card 3 -->
        <div class="relative bg-sky-100 p-6 rounded-lg shadow-md overflow-hidden">
          <h3 class="text-xl font-semibold mb-4">Édition Limitée</h3>
          <p class="text-sm text-gray-700 mb-4">
            Des créations uniques, disponibles pour une durée limitée seulement.
          </p>
          <NuxtLink to="/produit" class="text-sm font-medium text-gray-800 hover:underline">
            Voir la boutique
          </NuxtLink>
          <img
            src="/img/edition_limite.png"
            alt="Savon exclusif"
            class="absolute right-2 bottom-2 w-28 h-auto object-contain z-10"
          />
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
          <img src="/icons/ingredients.png" alt="" />
        </div>
        <h3 class="text-xl font-semibold text-gray-700 mb-2">Ingrédients Naturels</h3>
        <p class="text-gray-500">Des ingrédients purs pour une peau saine.</p>
      </div>
      <div class="p-6 bg-white rounded-md shadow-md">
        <div
          class="w-16 h-16 mx-auto bg-blue-200 text-blue-600 rounded-full flex items-center justify-center mb-4"
        >
          <img src="/icons/hand.png" alt="" />
        </div>
        <h3 class="text-xl font-semibold text-gray-700 mb-2">Fabrication Artisanale</h3>
        <p class="text-gray-500">Savons faits à la main avec soin.</p>
      </div>
      <div class="p-6 bg-white rounded-md shadow-md">
        <div
          class="w-16 h-16 mx-auto bg-yellow-200 text-yellow-600 rounded-full flex items-center justify-center mb-4"
        >
          <img src="/icons/dry-skin.png" alt="" />
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
          <NuxtLink to="/produit">
            <img src="/img/soap-1.jpg" alt="Savon 1" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Douceur</h3>
              <p class="text-gray-500 text-sm">Un savon doux pour une utilisation quotidienne.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/produit">
            <img src="/img/soap-2.jpg" alt="Savon 2" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Exfoliant</h3>
              <p class="text-gray-500 text-sm">Pour une peau lisse et renouvelée.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/produit">
            <img src="/img/soap-3.jpg" alt="Savon 3" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Parfumé</h3>
              <p class="text-gray-500 text-sm">Un parfum délicat pour une sensation agréable.</p>
            </div>
          </NuxtLink>
        </div>
        <div class="bg-gray-100 rounded-md shadow-md overflow-hidden">
          <NuxtLink to="/produit">
            <img src="/img/soap-4.jpg" alt="Savon 4" class="w-full h-48 object-cover" />
            <div class="p-4">
              <h3 class="text-lg font-semibold text-gray-700 mb-2">Savon Hydratant</h3>
              <p class="text-gray-500 text-sm">Pour une peau douce et hydratée.</p>
            </div>
          </NuxtLink>
        </div>
      </div>
      <!-- <div class="text-center mt-8">
        <NuxtLink
          to="/products"
          class="inline-block bg-green-500 hover:bg-green-600 text-white font-semibold py-3 px-6 rounded-full"
          >Voir Toute la Collection</NuxtLink
        >
      </div> -->
    </div>
  </section>

  <!-- <section class="py-12 bg-gray-50">
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
  </section> -->
</template>

<script setup lang="ts"></script>

<style scoped></style>
