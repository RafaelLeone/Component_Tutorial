<template>
  <div>
    <BCard>
      <img
        class="travel-card--image"
        src="https://cdn.greatsoftwares.com.br/arquivos/paginas_publicadas/gp.buser.com.br-pacotes/imagens/mobile/1661797641-8266086-4280-39b9fd009b6bb73ccecd1a45df6d4c7a.jpg"
      />
      <div class="travel-card--body">
        <h3 class="travel-card--title">{{ title }}</h3>
        <ul class="travel-card--description">
          <li v-for="(category, index) in categories" :key="index">
            {{ category }}
          </li>
        </ul>
        <BButton color="secondary">Meu botão</BButton>
        <BButton block>Meu botão 2</BButton>
      </div>
    </BCard>
  </div>
</template>

<script>
import BCard from "@/components/ui/atoms/b-card.vue";
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    categories: {
      type: Array,
      required: true,
    },
    image: {
      type: String,
      required: true,
    },
  },
  components: {
    BCard,
  },
};
</script>

<style>
.travel-card--image {
  margin: calc(-1 * 16px);
  width: calc(100% + 16px * 2);
  margin-bottom: 24px;
}
.travel-card--body {
}
.travel-card--title {
  text-align: left;
  margin-left: 16px;
  font-size: 19px;
}
.travel-card--description {
  text-align: left;
  font-size: 12px;
}
</style>
