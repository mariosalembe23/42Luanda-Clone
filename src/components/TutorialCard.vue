<script setup>
defineProps({
  tema: String,
  context: String,
  icon: String,
});
</script>
<template>
  <div
    class="cardTutorial p-3 rounded-md divide-x grid grid-cols-1 lg:grid-cols-5 items-center gap-3"
  >
    <header class="col-span-2">
      <div class="bg-zinc-950 p-3 rounded-md">
        <h6 class="text-white text-xl font-semibold">
          <i :class="icon"></i>
          {{ tema }}
        </h6>
      </div>
    </header>
    <main class="px-4  border-zinc-700 col-span-3 py-3">
      <p class="text-zinc-100 textTutorial">
        {{ context }}
      </p>
    </main>
  </div>
</template>

<style scoped>
.textTutorial {
  font-size: 15px;
}
</style>
