<template>
  <div>
    <nuxt-link :to="{ name:'index' }">Index</nuxt-link>
    <nuxt-link :to="{ name:'index', query: { test: 'test' } }">Index?test</nuxt-link>

    <nuxt-link :to="{ name:'route1' }">Route1</nuxt-link>
    <nuxt-link :to="{ name:'route1', query: { test: 'test' } }">Route1?test</nuxt-link>

    <nuxt-link :to="{ name:'route2' }">Route2</nuxt-link>
    <nuxt-link :to="{ name:'route2', query: { test: 'test' } }">Route2?test</nuxt-link>

    <slot />
  </div>
</template>
