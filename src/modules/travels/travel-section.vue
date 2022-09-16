<template>
  <div class="travel-section">
    <h2 class="travel-section--title">{{ title }}</h2>
    <div class="travel-section--grid">
      <TravelCard />
      <TravelCard />
      <TravelCard />
    </div>
  </div>
</template>

<script>
import TravelCard from "./travel-card.vue";

export default {
  components: {
    TravelCard,
  },
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style>
.travel-section {
}
.travel-section--grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
}
.travel-section--title {
  color: rgb(241, 16, 117);
}
</style>
