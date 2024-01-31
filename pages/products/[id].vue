<script setup lang="ts">
definePageMeta({
  layout: "products"
})
const {id} = useRoute().params
const uri = `https://fakestoreapi.com/products/${id}`;
const {data: product} = await useFetch(uri);
</script>

<template>
  <div>
    <ProductDetails :product="product"/>
  </div>
</template>