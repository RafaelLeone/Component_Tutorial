<template>
  <div class="travel-section">
    <TravelCard />
    <TravelCard />
    <TravelCard />
  </div>
</template>

<script>
import TravelCard from "./travel-card.vue"

export default {
 components: {
    TravelCard,
}
}
</script>

<style>
.travel-section {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
}
</style>