<template>
  <div class="">route1 {{ data }}</div>
</template>

<script setup>
const {
  data
} = await useAsyncData('page-route-1', () => $fetch('https://jsonplaceholder.typicode.com/posts/1', {method: 'get'}))
</script>
