<script setup>
defineProps({
  iconName: String,
  tittleText: String,
  text: String,
});
</script>

<template>
  <div
    class="p-5 bg-zinc-950 shadow-lg rounded-md cursor-pointer transition-all hover:ring-4 hover:ring-zinc-800 hover:ring-opacity-40"
  >
    <header class="w-full flex items-center space-x-2 pb-2">
      <i :class="iconName"></i>
      <h4 class="text-xl font-semibold text-zinc-300">{{ tittleText }}</h4>
    </header>
    <main>
      <p class="textDinamic text-white font-medium">
        {{ text }}
      </p>
    </main>
  </div>
</template>

<style scoped>
i {
  font-size: 1.3rem;
}
.textDinamic {
  font-size: 15px;
}
</style>
