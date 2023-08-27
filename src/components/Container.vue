<template>
  <Header />
  <main class="main mx-auto mt-12">
    <Topicos />
    <Vantagens />
  </main>
</template>

<script>
import Header from "./Header.vue";
import Topicos from "./Topicos.vue";
import Vantagens from "./Vantagens.vue";

export default {
  components: {
    Header,
    Topicos,
    Vantagens,
  },
};
</script>

<style scoped>
.main {
  max-width: 72rem;
  width: 100%;
}
</style>
