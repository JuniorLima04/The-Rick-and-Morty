<script setup>
const props = defineProps(["character"])
</script>

<template>
  <div class="col-md-4">
    <div class="card p-3 mb-4">
      <img :src="character.image" height="auto" alt="" class="rounded-circle mx-auto d-block">
      <div class="card-body text-center">
        <p class="mb-1"><strong>Nome:</strong> {{ character.name }}</p>
        <p class="mb-1"><strong>Status:</strong> {{ character.status }}</p>
        <p class="mb-1"><strong>Espécie:</strong> {{ character.species }}</p>
        <p class="mb-1"><strong>Gênero:</strong> {{ character.gender }}</p>
        <p class="mb-1"><strong>Localização:</strong> {{ character.location.name }}</p>
        <p class="mb-0"><strong>Episódios:</strong> {{ character.episode.length }}</p>
      </div>
    </div>
  </div>
</template>

