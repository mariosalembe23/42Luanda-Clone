<script setup>
defineProps({
  tittle: String,
  iconName: String,
  text: String
});
</script>

<template>
  <aside>
    <div class="bg-zinc-900 p-5 rounded-md h-44 grid grid-cols-6">
      <div
        class="col-span-2 rounded-md flex items-center justify-center bg-cyan-600"
      >
        <i :class="iconName"></i>
      </div>
      <div class="px-3 py-2 col-span-4">
        <h4 class="text-zinc-300 font-semibold">{{ tittle }}</h4>
        <p class="textInfo pt-1 text-white">
         {{ text }}
        </p>
      </div>
    </div>
  </aside>
</template>

<style scoped>
.iconVantagem {
  font-size: 2.5rem;
}
.textInfo {
  font-size: 14px;
}
</style>
