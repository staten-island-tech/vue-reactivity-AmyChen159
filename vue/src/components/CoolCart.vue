<template>
   <div class="cart">
      <h2>{{ Item.title }} - {{ Item.price }}</h2>
  </div>
</template>
  
<script setup>
const props = defineProps({
  Item: Object,
});

</script>

<style scoped>

</style>