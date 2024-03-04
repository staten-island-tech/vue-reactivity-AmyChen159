<template>
    <div class="cart-gallery">
      <Cart v-for="item in cartItems"
      :key="cartItems.title"
      :Item="item"
      />
    </div>
  
  </template>
  
  <script setup>
  import Cart from '@components/Cart.vue';
  import { cart } from '@/stores/cart.js';
  import { computed } from 'vue';

  const cartItems = computed(() => cart.value);
  </script>
  
  <style scoped>
  
  </style>