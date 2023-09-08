<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="b in blogs">
        <h2>
          <NuxtLink :to="`/products/${b.id}`">{{ b.title }}</NuxtLink>
        </h2>
      </div>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "blogs",
});
//  fetch data
const { data: blogs } = await useFetch("https://fakestoreapi.com/products");
</script>

<style scoped></style>
