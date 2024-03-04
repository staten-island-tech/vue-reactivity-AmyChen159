<template>
   <div class="cart">
      <h2>{{ Item.title }} - {{ Item.price }}</h2>
  </div>
</template>
  
<script setup>
import { computed } from "vue";
import { cart } from '@/stores/cart.js'; 

const cartItems = computed(() => cart.value);

const props = defineProps({
  Item: Object,
});

</script>

<style scoped>

</style>