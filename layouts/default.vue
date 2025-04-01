<template>
  <div>
    <header>
      <nav class="flex flex-row">
        <NuxtLink to="/">Les Savons Moussants</NuxtLink>
        <ul class="flex">
          <li><NuxtLink to="/">Home</NuxtLink></li>
          <li><NuxtLink to="/about">About</NuxtLink></li>
          <li><NuxtLink to="/products">Products</NuxtLink></li>
        </ul>
      </nav>
    </header>
  </div>

  <!-- page content -->
  <div>
    <slot></slot>
  </div>
</template>
