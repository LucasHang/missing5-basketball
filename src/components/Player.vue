<script lang="ts">
    import { RouterLink } from 'vue-router'

    export default {
        props: {
            player: Number,
        },
    }
</script>

<template>
  <div class="item">
    <i>
      <slot name="icon"></slot>
    </i>
    <div class="details">
      <h3>
        <slot name="heading"></slot>
      </h3>
      <RouterLink :to="`/guessing/${this.player}`">Adivinhar jogador</RouterLink>
    </div>
  </div>
</template>

<style scoped>
.item {
  display: flex;
  align-items: center;
}

.details {
  flex: 1;
  margin-left: 2rem;
}

i {
    display: flex;
    place-items: center;
    place-content: center;
    width: 100px;
    height: 100px;

    background: var(--color-border);
    border-radius: 8px;

    color: var(--color-text);

    padding: 0.5rem;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  color: var(--color-heading);
}
</style>
