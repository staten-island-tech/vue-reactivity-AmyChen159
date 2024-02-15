<template>
  <div>
    <BookCard v-for="book in books"
    :key="book.title"
    :Book="book"
    />
  </div>
</template>

<script setup>
import BookCard from '@/components/BookCard.vue'
const books = [
  {
    title: "Everything I Know About Love: A Memoir",
    author: "Dolly Alderton",
    version: "Paperback",
    price: "$18.99",
    genres: "Memoir, Biography, Autobiography, Humor",
    img: "./book1.jpg",
  },
  {
    title: "Good Material: A novel",
    author: "Dolly Alderton",
    version: "Hardcover",
    price: "$28.00",
    genres: "Humorous Fiction",
    img: "./book2.jpg",
  },
  {
    title: "A Litle Life",
    author: "Hanya Yanagihara",
    version: "Paperback",
    price: "$18.00",
    genres: "Novel",
    img: "./book3.jpg",
  },
  {
    title: "Bride",
    author: "Ali Hazelwood",
    version: "Paperback",
    price: "$19.00",
    genres: "Romance, Fantasy",
    img: "./book4.jpg",
  },
  {
    title: "A Court of Thorns and Roses (Book 1)",
    author: "Sarah J. Maas",
    version: "Paperback",
    price: "$19.00",
    genres: "Novel, Fantasy Fiction, Young adult literature, High fantasy",
    img: "./book5.jpg",
  },
  {
    title: "The Creative Act: A Way of Being",
    author: "Rick Rubin, Neil Strauss",
    version: "Hardcover",
    price: "$32.00",
    genres: "Self-help book",
    img: "./book6.jpg",
  },
  {
    title: "Martyr!: A novel",
    author: "Kaveh Akbar",
    version: "Hardcover",
    price: "$28.00",
    genres: "Urban fiction, LGBT literature",
    img: "./book7.jpg",
  },
  {
    title: "101 Essays That Will Change The Way You Think",
    author: "Brianna Wiest",
    version: "Paperback",
    price: "$15.99",
    genres: "Self-help book",
    img: "./book8.jpg",
  },
  {
    title: "The Bell Jar",
    author: "Sylvia Plath, (Foreword) Frances McCullough, (Illustrator) Sylvia Plath",
    version: "Paperback",
    price: "$17.99",
    genres: "Novel, Autobiography",
    img: "./book9.jpg",
  },
  {
    title: "How to Love (Mindfulness Essentials)",
    author: "Thich Nhat Hanh",
    version: "Paperback",
    price: "$9.95",
    genres: "Self-help book",
    img: "./book10.jpg",
  },
  {
    title: "I Never Knew That About New York",
    author: "Christopher Winn",
    version: "Paperback",
    price: "$18.00",
    genres: "Biography, Reference work, Travel literature",
    img: "./book11.jpg",
  },
  {
    title: "The Unbearable Lightness of Being",
    author: "Milan Kundera, (Translator) Michael Henry Heim",
    version: "Paperback",
    price: "$18.99",
    genres: "Novel, Magical Realism, Philosophical fiction",
    img: "./book12.jpg",
  },
  {
    title: "Everyone Who Can Forgive Me Is Dead: A Novel",
    author: "Jenny Hollander",
    version: "Hardcover",
    price: "$28.00",
    genres: "Thriller, Suspense, Psychological thriller",
    img: "./book13.jpg",
  },
  {
    title: "The Secret History",
    author: "Donna Tartt",
    version: "Paperback",
    price: "$18.00",
    genres: "Novel, Psychological Fiction",
    img: "./book14.jpg",
  },
  {
    title: "Subliminal: How Your Unconscious Mind Rules Your Behavior",
    author: "Leonard Mlodinow",
    version: "Paperback",
    price: "$17.00",
    genres: "Self-help book",
    img: "./book15.jpg",
  },
]
</script>

<style scoped>

</style>
