<template>
  <div class="">route2 {{ data }}</div>
</template>

<script setup>
const {
  data
} = await useAsyncData('page-route-2', () => $fetch('https://jsonplaceholder.typicode.com/posts/1', {method: 'get'}))
</script>
