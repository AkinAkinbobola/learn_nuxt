<script setup lang="ts">

</script>

<template>
  <div>
    <header class="shadow-sm mx-auto bg-white">
      <nav class="container p-4 mx-auto">
        <NuxtLink to="/products" class="font-bold">Nuxt Dojo Merch</NuxtLink>
      </nav>
    </header>

    <div class="container p-4 mx-auto">
      <slot/>
    </div>
    <footer class="container mx-auto p-4 border-t-2">
      <ul class="flex gap-4">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/products">Products</NuxtLink>
        </li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: #12b488;
}
</style>