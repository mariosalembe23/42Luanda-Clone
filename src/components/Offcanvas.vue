<script setup>
function closeOffCanvas() {
  const offCanvas = document.querySelector(".offcanvas");

  offCanvas.classList.remove("showOffCanvas");
  document.body.style.overflow = 'auto'
}
</script>
<template>
  <div class="offcanvas z-30 p-6 relative lg:hidden inline-block">
    <header class="flex items-center w-full justify-between">
      <span class="menu text-white font-semibold text-xl">Menu</span>
      <button class="text-2xl" @click="closeOffCanvas">
        <i class="bi bi-arrow-bar-right text-red-300"></i>
      </button>
    </header>
    <main class="mt-8">
      <nav>
        <ul class="flex flex-col space-y-6">
          <li class="flex items-center justify-between w-full">
            <a
            @click="closeOffCanvas"
              href="#topicos"
              class="offLink transition-all hover:text-white text-cyan-100 font-medium"
              >Sobre</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
            @click="closeOffCanvas"
              href="#vantagens"
              class="offLink transition-all hover:text-white text-cyan-100 font-medium"
              >Vantagens</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
            @click="closeOffCanvas"
              href="#comunidade"
              class="offLink transition-all hover:text-white text-cyan-100 font-medium"
              >Comunidade</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
            @click="closeOffCanvas"
              href="#FAQ"
              class="offLink transition-all hover:text-white text-cyan-100 font-medium"
              >FAQ</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
        </ul>
      </nav>
      <div class="absolute right-0 bottom-4 w-full px-4">
        <a
          href="#"
          class="offLogin text-zinc-800 block bg-cyan-400 py-3 rounded-md font-semibold text-center transition-all hover:bg-cyan-300"
          >Faça Login</a
        >
      </div>
    </main>
  </div>
</template>
<style scoped>
.offcanvas {
  backdrop-filter: blur(10px);
  background-color: rgba(0, 0, 0, 0.7);
  position: fixed;
  top: 0;
  right: 0;
  width: 60%;
  height: 100vh;
  transform: translateX(40rem);
  transition: transform 0.34s ease-in-out;
}
.showOffCanvas {
  transform: translateX(0rem) !important;
}
.menu,
.offLink {
  font-family: "Poppins", sans-serif;
}
.offLogin {
  font-family: "Poppins", sans-serif;
  font-size: 15px;
}
@media screen and (max-width:640px) {
    .offcanvas{
        width: 100vw;
    }
}
</style>
