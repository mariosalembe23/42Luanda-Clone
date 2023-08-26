<template>
  <Header />
  <main class="main mx-auto mt-12">
    <Topicos />
  </main>
</template>

<script>
import Header from "./Header.vue";
import Topicos from "./Topicos.vue";

export default {
  components: {
    Header,
    Topicos,
  },
};
</script>

<style scoped>
.main {
  max-width: 72rem;
  width: 100%;
}
</style>
