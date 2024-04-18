<template>
  <div>
    <header class="bg-white shadow-sm">
      <nav class="flex justify-between container p-4 mx-auto">
        <NuxtLink
          to="/"
          class="font-bold text-red-600 hover:text-green-900 transition-all duration-100 ease-linear"
          >NUXT <span class="text-green-600">PROJECT</span></NuxtLink
        >
        <ul class="flex gap-4">
          <li>
            <NuxtLink
              to="/"
              class="font-bold hover:text-green-600 transition-all duration-100 ease-linear"
              >Home</NuxtLink
            >
          </li>
          <li>
            <NuxtLink
              to="/about"
              class="font-bold hover:text-green-600 transition-all duration-100 ease-linear"
              >About</NuxtLink
            >
          </li>
          <li>
            <NuxtLink to="/products" class="btn">Products</NuxtLink>
          </li>
        </ul>
      </nav>
    </header>
  </div>
  <div class="container mx-auto p-4">
    <slot />
  </div>
</template>

<script setup></script>

<style scoped>
.router-link-exact-active {
  color: green;
}
</style>
