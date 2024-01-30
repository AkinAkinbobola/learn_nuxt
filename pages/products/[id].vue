<script setup lang="ts">
const {id} = useRoute().params
definePageMeta({
  layout: "products"
})
</script>

<template>
  <div>
    <p>Product details for product {{ id }}</p>
  </div>
</template>