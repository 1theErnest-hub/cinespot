<script setup>
defineProps({
    movie: Object
})
</script>

<template>
    <div class="card">
        <img :src="`/posters/${movie.id}.jpg`" :alt="movie.title" />
        <h3>{{ movie.title }}</h3>
        <p>{{ movie.genre }}</p>
    </div>
</template>

<style scoped>

.card{
    background:#1f2937;
    border-radius:10px;   /*Es para un borde redondo*/
    padding: 11px;          /*Es para el espacio interno*/

}
img {
  width: 100%;
  aspect-ratio: 2 / 3;
  object-fit: cover;
  border-radius: 8px;
}

</style>