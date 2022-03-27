<script lang="ts">
    export default {
        created() {
            console.log(this.$route.params.playerNumber)
        }
    }
</script>

<template>
  <div class="guessing">
    <h1>This is an guessing page</h1>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .guessing {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
