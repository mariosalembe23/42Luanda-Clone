<template>
  <Header />
  <main class="main mx-auto mt-12">
    <Topicos />
    <Vantagens />
    <Comunidade/>
    <FAQ/>
  </main>
</template>

<script>
import Header from "./Header.vue";
import Topicos from "./Topicos.vue";
import Vantagens from "./Vantagens.vue";
import Comunidade from "./Comunidade.vue";
import FAQ from './FAQ.vue'

export default {
  components: {
    Header,
    Topicos,
    Vantagens,
    Comunidade,
    FAQ
  },
};
</script>

<style scoped>
.main {
  max-width: 72rem;
  width: 100%;
}
</style>
