<script>
export default {
  props: {
    question: String,
    response: String,
  },
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    closeContainer() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
<template>
  <div
    @click="closeContainer"
    class="w-full py-3 px-4 bg-zinc-900 transition-all hover:bg-zinc-800 rounded-sm cursor-pointer flex items-center justify-between"
  >
    <p class="font-semibold question text-white text-start">{{ question }}</p>
    <button id="" class="text-xl text-cyan-300 signal">
      <span v-if="!isOpen">+</span>
      <span v-else>-</span>
    </button>
  </div>
  <div class="px-4 py-1 container" v-show="isOpen">
    <p class="textAccordion font-medium text-white">
      {{ response }}
    </p>
  </div>
</template>
<style scoped>
.question {
  font-family: "Poppins", sans-serif;
}
.textAccordion {
  font-size: 15px;
}
.container {
  overflow: hidden;
  transition: all 0.5s ease-in-out;
}
</style>
