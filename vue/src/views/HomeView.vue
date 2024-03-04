<template>
  <div class="gallery">
    <BookCard v-for="book in books"
    :key="book.title"
    :Book="book"
    />
  </div>
</template>

<script setup>
import BookCard from '@/components/BookCard.vue';
import { useBooks } from '@/stores/cart';

const books = useBooks().books

</script>

<style scoped>

.gallery {
  display: flex;
  flex-wrap: wrap; 
  justify-content: space-around;
}

</style>
