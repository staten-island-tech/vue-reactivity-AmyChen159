<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header >
     <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/cart">Cart</RouterLink>
      </nav>
  </header>

  <RouterView />
</template>

<style scoped>

</style>
