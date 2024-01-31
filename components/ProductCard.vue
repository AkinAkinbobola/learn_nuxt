<script setup lang="ts">
const {product} = defineProps(["product"])
</script>

<template>
<div class="card text-center">
  <img :src="product.image" class="thumb" alt="Product thumb">
  <p class="font-bold text-gray-500 m-4 truncate">{{product.title}}</p>
  <NuxtLink :to="`/products/${product.id}`">
    <p class="btn my-4">
      View Details
    </p>
  </NuxtLink>
</div>
</template>

<style scoped>

</style>