<template>
  <div>
    <AppHeader />
    <AppMain />
    <TravelSection
      v-for="(cidade, index) in cidades"
      :key="index"
      :title="`Pacotes de viagens saindo de ${cidade.name}`"
    />
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
  data() {
    return {
      cidades: [
        {
          name: "São Paulo",

          destinos: [
            {
              name: "Rio de Janeiro",
            },
            {
              name: "Campos do Jordão",
            },
            {
              name: "Caçapava",
            },
          ],
        },
        {
          name: "Rio de Janeiro",

          destinos: [
            {
              name: "Taubaté",
            },
            {
              name: "Ubatuba",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
