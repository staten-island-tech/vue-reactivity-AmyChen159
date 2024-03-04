<template>
  <h1>Items in Cart</h1>
  <div class="cart">
    <h2 v-for="item in cartItems" :key="item.title">{{ item.title }}</h2>
    <h3 v-for="item in cartItems" :key="item.title">{{ item.price }}</h3>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { cartItems } from '@/stores/cart.js'; // Assuming you have a store for cart items

// If you're not using a store, you can pass the cart items as props
// const props = defineProps({
//   cartItems: Array
// })
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>

