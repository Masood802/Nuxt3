<template>
  <div class="card text-center">
    <img :src="product.image" alt="Image" class="thumb" />
    <p class="font-bold m-4 text-gray-500 truncate">{{ product.title }}</p>
    <NuxtLink :to="`/products/${product.id}`"
      ><p class="btn my-4">View Details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
.thumb {
  max-height: 125px;
  max-width: 75%;
  margin: 0 auto;
}
</style>
