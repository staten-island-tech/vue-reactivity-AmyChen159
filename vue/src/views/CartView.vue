<template>
    <div class="cart-gallery">
      <CoolCart v-for="item in store.cart"
      :Item="item">
      </CoolCart>
    </div>
  </template>
  
  <script setup>

  import CoolCart from '@/components/CoolCart.vue';
  import { useCart } from '@/stores/cart.js';

  const store = useCart()

  </script>
  
  <style scoped>
  
  </style>