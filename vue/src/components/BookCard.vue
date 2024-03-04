<template>
    <div class="cards">
        <h2>{{ Book.title }}</h2>
        <h3>By: {{ Book.author }}</h3>
        <img :src="Book.img" alt="" />
        <h3>Price: {{ Book.price }}</h3>
        <h3>{{ Book.clicked }} Item(s) in Cart</h3>
        <button @click="addCart(Book)">Add to Cart</button>
    </div> 
</template>

<script setup>
import { useCart } from '@/stores/cart.js';

const store = useCart();

const props = defineProps({
  Book: Object,
});

function addCart(Item) {
  Item.clicked++;
  store.cart.push(Item);
  console.log(store.cart);
}
</script>

<style scoped>

.cards {
  padding: 3%;
  margin: 2%;
  justify-content: space-between;
  overflow-wrap: break-word;
  max-width: 300px;
  align-items: center;
}

img { 
  width: 300px;
  height: 400px;
}

</style>