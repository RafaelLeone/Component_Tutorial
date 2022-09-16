<template>
  <div>
    <AppHeader />
    <AppMain />
    <TravelSection />
  </div>
</template>

<script>
import AppMain from "../components/app/app-main.vue";
import AppHeader from "../components/app/app-header.vue";
import TravelSection from "@/modules/travels/travel-section.vue";

export default {
  components: {
    AppMain,
    AppHeader,
    TravelSection,
},
};
</script>

<style></style>
