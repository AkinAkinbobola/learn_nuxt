<script setup lang="ts">

definePageMeta({
  layout: "products"
})
useHead({
  title: "Nuxt Dojo | Merch",
  meta: [
    {
      name: "description",
      content: "Nuxt 3 Merch"
    }
  ]
})
const {data: products} = await useFetch('https://fakestoreapi.com/products');

</script>

<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="(product) in products" :key="product.id">
        <ProductCard :product="product"/>
      </div>
    </div>
  </div>
</template>