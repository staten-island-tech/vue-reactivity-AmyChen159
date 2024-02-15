<template>
    <div>
        <h1>{{ Book.name }}</h1>
        <img :src="Book.img" alt="" />
        <h2>{{ clicked }}</h2>
        <button @click="increment">Click Me !</button>
    </div>
</template>

<script setup>
import { ref } from "vue";
const props = defineProps({
  Book: Object,
});

const clicked = ref(0);
function increment() {
  clicked.value++;
}
</script>

<style scoped>
img { 
  width: 250px;
  height: 300px;
  object-fit: cover;
}
</style>