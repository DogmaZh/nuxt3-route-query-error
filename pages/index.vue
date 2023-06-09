<template>
  <div class="">index {{ data }}</div>
</template>

<script setup>
const {
  data
} = await useAsyncData('page-index', () => $fetch('https://jsonplaceholder.typicode.com/posts/1', {
  method: 'get'}))
</script>
