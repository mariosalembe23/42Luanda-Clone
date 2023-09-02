<script setup>
function closeOffCanvas() {
  const offCanvas = document.querySelector(".offcanvas");

  offCanvas.classList.remove("showOffCanvas");
  document.body.style.overflow = "auto";
}

function SpecialFunction() {
  const offCanvas = document.querySelector(".offcanvas");
  const messageComponent = document.querySelector(".back");
  const CardMessage = document.querySelector(".card-message");
  messageComponent.classList.remove("hidden");
  CardMessage.classList.add("showCardMessage");
  offCanvas.classList.remove("showOffCanvas");
  document.body.style.overflow = "auto";
}
</script>
<template>
  <div class="offcanvas z-30 p-6 relative lg:hidden inline-block">
    <header class="flex items-center w-full justify-between">
      <span class="menu text-white font-semibold text-xl">Menu</span>
      <button class="text-red-200" @click="closeOffCanvas">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-6 h-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>
      </button>
    </header>
    <main class="mt-8">
      <nav>
        <ul class="flex flex-col space-y-6">
          <li class="flex items-center justify-between w-full">
            <a
              @click="closeOffCanvas"
              href="#topicos"
              class="offLink transition-all hover:text-white text-cyan-50 font-medium flex items-center gap-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M17.593 3.322c1.1.128 1.907 1.077 1.907 2.185V21L12 17.25 4.5 21V5.507c0-1.108.806-2.057 1.907-2.185a48.507 48.507 0 0111.186 0z"
                />
              </svg>

              Sobre</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
              @click="closeOffCanvas"
              href="#vantagens"
              class="offLink transition-all hover:text-white text-cyan-50 font-medium flex items-center gap-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M3.75 13.5l10.5-11.25L12 10.5h8.25L9.75 21.75 12 13.5H3.75z"
                />
              </svg>

              Vantagens</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
              @click="closeOffCanvas"
              href="#comunidade"
              class="offLink transition-all hover:text-white text-cyan-50 font-medium flex items-center gap-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M18 18.72a9.094 9.094 0 003.741-.479 3 3 0 00-4.682-2.72m.94 3.198l.001.031c0 .225-.012.447-.037.666A11.944 11.944 0 0112 21c-2.17 0-4.207-.576-5.963-1.584A6.062 6.062 0 016 18.719m12 0a5.971 5.971 0 00-.941-3.197m0 0A5.995 5.995 0 0012 12.75a5.995 5.995 0 00-5.058 2.772m0 0a3 3 0 00-4.681 2.72 8.986 8.986 0 003.74.477m.94-3.197a5.971 5.971 0 00-.94 3.197M15 6.75a3 3 0 11-6 0 3 3 0 016 0zm6 3a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0zm-13.5 0a2.25 2.25 0 11-4.5 0 2.25 2.25 0 014.5 0z"
                />
              </svg>

              Comunidade</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <a
              @click="closeOffCanvas"
              href="#FAQ"
              class="offLink transition-all hover:text-white text-cyan-50 font-medium flex items-center gap-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M9.879 7.519c1.171-1.025 3.071-1.025 4.242 0 1.172 1.025 1.172 2.687 0 3.712-.203.179-.43.326-.67.442-.745.361-1.45.999-1.45 1.827v.75M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-9 5.25h.008v.008H12v-.008z"
                />
              </svg>

              FAQ</a
            >
            <i class="bi bi-chevron-right text-cyan-100"></i>
          </li>
          <li class="flex items-center justify-between w-full">
            <button
              @click="SpecialFunction"
              href="#"
              class="offLink transition-all hover:text-white text-cyan-50 font-medium flex items-center gap-2"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0M3.124 7.5A8.969 8.969 0 015.292 3m13.416 0a8.969 8.969 0 012.168 4.5"
                />
              </svg>

              Notificações</button
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
@media screen and (max-width: 640px) {
  .offcanvas {
    width: 100vw;
  }
}
</style>
