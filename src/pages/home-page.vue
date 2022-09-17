<template>
  <div>
    <AppHeader />
    <AppMain />
    <TravelSection
      v-for="(cidade, index) in cidades"
      :key="index"
      :title="`Pacotes de viagens saindo de ${cidade.name}`"
      :cidades="cidade.destinos"
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
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-8266086-4280-39b9fd009b6bb73ccecd1a45df6d4c7a.jpg",
            },
            {
              name: "Campos do Jordão",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/desktop/1661797641-7354692-4280-8940d8ea40163939ab19d95a586b5c7c.jpg",
            },
            {
              name: "Aparecida",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-7354701-4280-ad3c046a884c2fb3feb26f96f1d8165d.jpg",
            },
          ],
        },
        {
          name: "Rio de Janeiro",

          destinos: [
            {
              name: "São Paulo",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-7354739-4280-1ab4d2499353bdfe09458c32c58f8f2b.jpg",
            },
            {
              name: "Campos do Jordão",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-7354730-4280-02387372ad6c227a74aa19e1d952f8e3.jpg",
            },
            {
              name: "Búzios",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-8076743-4280-a5eb25cd0a73beb074ca6b932c18b0ae.jpg",
            },
          ],
        },
        {
          name: "Belo Horizonte",

          destinos: [
            {
              name: "Poços de Caldas",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-7354895-4280-612533168e1411bec58f6af62755988d.jpg",
            },
            {
              name: "Rio de Janeiro",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-8266086-4280-39b9fd009b6bb73ccecd1a45df6d4c7a.jpg",
            },
            {
              name: "São Paulo",
              image:
                "https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-7354739-4280-1ab4d2499353bdfe09458c32c58f8f2b.jpg",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style></style>
