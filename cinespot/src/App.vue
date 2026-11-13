<script setup>
import { movies } from './data/movies'; 
import MovieCard from './components/MovieCard.vue'


</script>

<template>

  <h1>CineSpot</h1>
  <div class="grid">
 <MovieCard v-for="movie in movies" :key="movie.id" :movie="movie" />
</div>
</template>

<style>

body {
  background: #111827;
  color: white;
  font-family: sans-serif;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
  gap: 16px;
}

</style>

