<template>
    <div class="cart-gallery">
      <Cart v-for="item in store.cart"
      :Item="item">
      </Cart>
    </div>
  
  </template>
  
  <script setup>
  import Cart from '@components/Cart.vue';
  import { useCart } from '@/stores/cart.js';
  const store = useCart()

  </script>
  
  <style scoped>
  
  </style>