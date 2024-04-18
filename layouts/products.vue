<template>
  <div>
    <header class="bg-white shadow-sm">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/products" class="font-bold">Products</NuxtLink>
      </nav>
    </header>
  </div>
  <div class="container mx-auto p-4">
    <slot />
  </div>
  <footer class="container mx-auto p-4 flex justify-between border-t-2">
    <ul>
      <li><NuxtLink to="/">Home</NuxtLink></li>
      <li><NuxtLink to="/about">About</NuxtLink></li>
      <li><NuxtLink to="/products">Products</NuxtLink></li>
    </ul>
  </footer>
</template>

<script setup></script>

<style scoped>
.router-link-exact-active {
  color: green;
}
</style>
