<template>
  <div>
    <p>{{ product.id }}</p>
    <p>{{ product.title }}</p>
    <p>{{ product.price }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
definePageMeta({
  layout: "products",
});
const url = "https://fakestoreapi.com/products/" + id;
const { data: product } = await useFetch(url, { key: id });
</script>

<style scoped></style>
