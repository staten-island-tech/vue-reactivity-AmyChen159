<template>
    <div class="cards">
        <h2>{{ Book.title }}</h2>
        <h3>By: {{ Book.author }}</h3>
        <img :src="Book.img" alt="" />
        <h3>{{ clicked }} Item(s) in Cart</h3>
        <button @click="addCart">Add to Cart</button>
    </div>
</template>

<script setup>
import { ref } from "vue";
const props = defineProps({
  Book: Object,
});

const clicked = ref(0);
function addCart() {
  clicked.value++;
}
</script>

<style scoped>
img { 
  width: 300px;
  height: 400px;
}

h1 {
  align-items: center;
}
</style>