<template>
   <div class="cart">
    <h2 v-for="item in cartItems" :key="item.title">{{ item.title }}</h2>
    <h3 v-for="item in cartItems" :key="item.title">{{ item.price }}</h3>
  </div>
</template>
  
<script setup>
import { computed } from "vue";
import { cart } from '@/stores/cart.js'; 
  
const cartItems = computed(() => cart.value);

</script>

<style scoped>

</style>