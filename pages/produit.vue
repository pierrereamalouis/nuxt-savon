<template>
  <section class="bg-white py-16 px-6 md:px-12">
    <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-12 items-start">
      <!-- Product Image -->
      <div class="bg-emerald-50 rounded-xl p-6 shadow-md">
        <img
          src="/img/soap-2.jpg"
          alt="Savon à l’eucalyptus"
          class="w-full h-auto object-contain rounded-md"
        />
      </div>

      <!-- Product Info -->
      <div class="space-y-6">
        <h1 class="text-3xl font-bold text-gray-900">Savon à l’Eucalyptus</h1>
        <p class="text-gray-700 text-lg">
          Un savon doux, purifiant et revigorant pour une peau propre et rafraîchie.
        </p>

        <div class="text-xl font-semibold text-emerald-800">8.50$</div>

        <div class="text-sm text-gray-600">
          <span class="font-semibold">Type :</span> Sans parabène<br />
          <span class="font-semibold">Vendeur :</span> Les Mains Moussantes
        </div>

        <div class="flex gap-4">
          <div>
            <p class="font-medium text-gray-700 mb-1">Poids</p>
            <div
              class="bg-emerald-100 text-emerald-900 px-4 py-2 rounded-full font-semibold text-sm w-fit"
            >
              100 g
            </div>
          </div>

          <div>
            <p class="font-medium text-gray-700 mb-1">Parfum</p>
            <div
              class="bg-emerald-100 text-emerald-900 px-4 py-2 rounded-full font-semibold text-sm w-fit"
            >
              Eucalyptus
            </div>
          </div>
        </div>

        <!-- Quantity Selector -->
        <div>
          <p class="font-medium text-gray-700 mb-1">Quantité</p>
          <div class="flex items-center gap-2 border border-gray-300 w-fit rounded-md px-2 py-1">
            <button class="text-lg font-semibold text-gray-600">−</button>
            <span class="w-6 text-center">1</span>
            <button class="text-lg font-semibold text-gray-600">+</button>
          </div>
        </div>

        <!-- Buttons -->
        <div class="flex flex-col sm:flex-row gap-4 mt-6">
          <button
            class="bg-emerald-700 hover:bg-emerald-800 text-white font-medium py-3 px-6 rounded-md"
          >
            Ajouter au panier
          </button>
          <button
            class="bg-white border border-emerald-300 hover:bg-emerald-50 text-emerald-700 font-medium py-3 px-6 rounded-md"
          >
            Ajouter à la liste de souhaits
          </button>
        </div>

        <button
          class="mt-4 w-full bg-emerald-100 hover:bg-emerald-200 text-emerald-800 font-semibold py-3 px-6 rounded-md text-center"
        >
          Acheter maintenant
        </button>

        <!-- Delivery Note -->
        <div class="text-sm text-gray-500 flex items-center gap-2 mt-4">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            class="w-5 h-5 text-gray-400"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="1.5"
              d="M3 10h1l3 9h13M5 10h16l-1.5-4.5H6.5L5 10z"
            />
          </svg>
          Livraison estimée dans 5 à 7 jours
        </div>
      </div>
    </div>
  </section>

  <section class="py-12 px-6 md:px-12 bg-white border-t">
    <div class="max-w-4xl mx-auto">
      <!-- Tabs Header -->
      <div class="flex space-x-4 border-b mb-6">
        <button
          v-for="tab in tabs"
          :key="tab.name"
          @click="activeTab = tab.name"
          :class="[
            'py-2 px-4 text-sm font-medium transition',
            activeTab === tab.name
              ? 'text-emerald-700 border-b-2 border-emerald-600 bg-emerald-50'
              : 'text-gray-500 hover:text-emerald-600',
          ]"
        >
          {{ tab.label }}
        </button>
      </div>

      <!-- Tabs Content -->
      <div class="space-y-6 text-gray-800 leading-relaxed">
        <!-- Description -->
        <div v-if="activeTab === 'description'">
          <p class="text-gray-800 leading-relaxed mb-4">
            Offrez à votre peau un moment de pure douceur avec notre savon artisanal à base
            d’ingrédients 100% naturels soigneusement sélectionnés pour leurs vertus hydratantes,
            protectrices et apaisantes.
          </p>

          <p class="text-gray-800 leading-relaxed mb-4">
            Enrichi en <strong>huile de coco</strong>, ce savon aide à retenir l’humidité naturelle
            de la peau tout en la maintenant souple et nourrie. Le <strong>beurre de cacao</strong>,
            riche en acides gras et en antioxydants, contribue à régénérer et protéger la peau
            contre les agressions extérieures.
          </p>

          <p class="text-gray-800 leading-relaxed mb-4">
            Grâce au <strong>beurre de karité</strong>, aux propriétés ultra-hydratantes, ce savon
            est un allié de choix pour les peaux sèches, sensibles ou déshydratées. L’<strong
              >huile d’olive</strong
            >, quant à elle, est naturellement riche en vitamines A et E, offrant une action
            anti-âge tout en améliorant l’élasticité de la peau.
          </p>

          <p class="text-gray-800 leading-relaxed">
            Nous y avons ajouté des huiles essentielles de <strong>lavande</strong> pour leurs
            propriétés antibactériennes et antifongiques, et de <strong>eucalyptus</strong> pour
            apaiser les rougeurs, réduire les gonflements et procurer une sensation de fraîcheur.
          </p>

          <p class="text-gray-800 leading-relaxed font-medium">
            Résultat : une peau propre, douce, hydratée et visiblement plus saine — naturellement.
          </p>
          <!-- Add the rest of the description from Step 1 -->
        </div>

        <!-- Shipping & Returns -->
        <div v-if="activeTab === 'shipping'">
          <h3 class="font-semibold text-lg">Politique de retour</h3>
          <p class="text-gray-800 leading-relaxed mb-4">
            Vous pouvez retourner la plupart des articles non utilisés dans un délai de 30 jours
            après la livraison pour un remboursement complet. Si le retour est dû à une erreur de
            notre part (produit incorrect ou défectueux), nous prenons en charge les frais
            d’expédition du retour.
          </p>

          <p class="text-gray-800 leading-relaxed mb-4">
            Une fois le colis reçu, le remboursement est généralement traité dans un délai de 3 à 5
            jours ouvrables. Le temps de traitement bancaire peut ensuite prendre 5 à 10 jours
            supplémentaires avant que le montant apparaisse sur votre compte.
          </p>

          <p class="text-gray-800 leading-relaxed mb-4">
            Pour effectuer un retour, connectez-vous à votre compte, accédez à votre commande via la
            section « Mes commandes », puis cliquez sur « Retourner un article ». Une notification
            par courriel vous sera envoyée dès que le remboursement aura été traité.
          </p>

          <h3 class="text-lg font-semibold text-gray-800 mt-8">Informations sur la livraison</h3>
          <p class="text-gray-800 leading-relaxed">
            Nous livrons partout dans le monde. Veuillez noter que certaines restrictions peuvent
            s’appliquer selon le type de produit ou le pays de destination.
          </p>

          <p class="text-gray-800 leading-relaxed">
            Lors de votre commande, nous estimons le délai de traitement et de livraison en fonction
            de la disponibilité de vos articles et du mode de livraison sélectionné. Ces estimations
            apparaîtront sur la page de paiement avant validation.
          </p>

          <p class="text-gray-800 leading-relaxed">
            Les frais d’expédition sont calculés selon le poids total des articles commandés. Pour
            respecter les politiques des transporteurs, les poids sont arrondis à l’unité
            supérieure.
          </p>
        </div>

        <!-- Reviews -->
        <div v-if="activeTab === 'reviews'">
          <p>Aucun avis pour le moment. Soyez le premier à partager votre expérience !</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
  // import { ref } from '@vue';

  const activeTab = ref('description');

  const tabs = [
    { name: 'description', label: 'Description' },
    { name: 'shipping', label: 'Expédition & Retours' },
    // { name: 'reviews', label: 'Avis' },
  ];
</script>

<style scoped></style>
