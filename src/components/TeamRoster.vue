<script setup lang="ts">
import Player from './Player.vue'
import AnonymousPlayer from './icons/AnonymousPlayer.vue'
</script>

<template>
  <Player :player=1>
    <template #icon><AnonymousPlayer /></template>
    <template #heading>Jogador 1</template>
  </Player>
  <Player :player=2>
    <template #icon><AnonymousPlayer /></template>
    <template #heading>Jogador 2</template>
  </Player>
</template>
