<template>
  <div class="min-h-screen flex flex-col">
    <header class="bg-white py-4 px-6 shadow-md">
      <div class="container mx-auto flex items-center justify-between">
        <div class="flex-shrink-0">
          <NuxtLink to="/" class="flex items-center space-x-3">
            <img src="/img/logo.png" alt="Les Mains Moussantes" class="h-14 w-auto" />
            <span class="font-sans text-lg font-semibold text-gray-800 whitespace-nowrap">
              Les Mains Moussantes
            </span>
          </NuxtLink>
        </div>
        <nav class="flex-grow">
          <ul class="flex justify-center space-x-8">
            <li>
              <NuxtLink to="/" class="font-sans text-gray-700 hover:text-gray-900">Accueil</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about" class="font-sans text-gray-700 hover:text-gray-900">À propos</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/products" class="font-sans text-gray-700 hover:text-gray-900"
                >Nos Produits</NuxtLink
              >
            </li>
          </ul>
        </nav>

        <div class="flex items-center space-x-4">
          <button class="text-gray-600 hover:text-gray-800 focus:outline-none">
            <svg
              class="h-6 w-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
              ></path>
            </svg>
          </button>
          <NuxtLink to="/login" class="text-gray-600 hover:text-gray-800 focus:outline-none">
            <svg
              class="h-6 w-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
              ></path>
            </svg>
          </NuxtLink>
          <NuxtLink
            to="/cart"
            class="relative text-gray-600 hover:text-gray-800 focus:outline-none"
          >
            <svg
              class="h-6 w-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </NuxtLink>
        </div>
      </div>
    </header>

    <!-- page content -->
    <main class="flex-grow">
      <NuxtPage />
    </main>

    <footer class="bg-gray-100 py-8 px-6 mt-8">
      <div
        class="container mx-auto grid grid-cols-1 md:grid-cols-3 lg:grid-cols-4 gap-8 text-gray-600"
      >
        <div>
          <h3 class="font-semibold text-gray-800 mb-4">À Propos</h3>
          <p class="text-sm">Brève description de votre entreprise.</p>
        </div>
        <div>
          <h3 class="font-semibold text-gray-800 mb-4">Boutique</h3>
          <ul class="space-y-2 text-sm">
            <li><NuxtLink to="/products">Tous les produits</NuxtLink></li>
            <li><NuxtLink to="/products?type=soaps">Savons</NuxtLink></li>
          </ul>
        </div>
        <div>
          <h3 class="font-semibold text-gray-800 mb-4">Informations</h3>
          <ul class="space-y-2 text-sm">
            <li><NuxtLink to="/contact">Contactez-nous</NuxtLink></li>
            <li><NuxtLink to="/privacy">Politique de confidentialité</NuxtLink></li>
            <li><NuxtLink to="/terms">Conditions d'utilisation</NuxtLink></li>
          </ul>
        </div>
        <div>
          <h3 class="font-semibold text-gray-800 mb-4">S'inscrire</h3>
          <p class="text-sm">Restez informé(e) de nos dernières nouvelles et offres.</p>
          <div class="mt-2">
            <input
              type="email"
              placeholder="Votre adresse courriel"
              class="w-full p-2 rounded-md border border-gray-300 text-sm"
            />
            <button
              class="bg-green-500 hover:bg-green-600 text-white py-2 px-4 rounded-md mt-2 text-sm"
            >
              S'inscrire
            </button>
          </div>
        </div>
      </div>
      <div class="mt-8 text-center text-gray-500 text-xs">
        &copy; {{ new Date().getFullYear() }} Votre Entreprise. Tous droits réservés.
      </div>
      <!-- <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/pixel-perfect" title="Pixel perfect"
          >Pixel perfect</a
        >
        from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/eucalyp" title="Eucalyp">Eucalyp</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/flat-icons" title="Flat Icons">Flat Icons</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/ilham-fitrotul-hayat" title="Ilham Fitrotul Hayat"
          >Ilham Fitrotul Hayat</a
        >
        from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/hilmy-abiyyu-a" title="Hilmy Abiyyu A."
          >Hilmy Abiyyu A.</a
        >
        from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/surang" title="surang">surang</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/gungyoga04" title="gungyoga04">gungyoga04</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/zero-wing" title="zero_wing">zero_wing</a> from
        <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/aziz-muttaqin" title="Aziz Muttaqin"
          >Aziz Muttaqin</a
        >
        from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div>
      <div>
        Icons made by
        <a href="https://www.flaticon.com/authors/egorpolyakov" title="egorpolyakov"
          >egorpolyakov</a
        >
        from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>
      </div> -->
    </footer>
  </div>
</template>
