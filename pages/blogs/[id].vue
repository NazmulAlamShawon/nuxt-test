<template>
  <div>
    <h2>{{ product.title }}</h2>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = `https://fakestoreapi.com/products` + id;
const { data: blog } = await useFetch(uri);
definePageMeta({
  layout: "blogs",
});
</script>

<style scoped></style>
