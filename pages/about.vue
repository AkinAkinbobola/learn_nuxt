<script setup lang="ts">
const {data} = useFetch("/api/ninja?name=SUPERSS", {
  method: "post",
  body: {
    age: 20
  }
})
</script>

<template>
  <div>
    <h1 class="font-bold">About</h1>
    <div>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. A adipisci dolorum et modi mollitia ratione saepe
      sapiente, ut vel voluptas.
    </div>
  </div>
</template>

<style scoped>

</style>