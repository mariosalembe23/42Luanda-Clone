<template>
  <aside
    class="back fixed top-0 left-0 right-0 w-full h-screen z-50 px-5 hidden"
  >
    <div
      class="card-message max-w-xl rounded-md w-full mx-auto my-8 p-5 bg-zinc-900"
    >
      <header
        class="flex items-center justify-between border-b border-zinc-800 pb-4"
      >
        <div class="flex items-center space-x-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-5 h-5 text-cyan-400"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0M3.124 7.5A8.969 8.969 0 015.292 3m13.416 0a8.969 8.969 0 012.168 4.5"
            />
          </svg>
          <p class="text-zinc-100 font-medium">Notificações</p>
        </div>
        <button
          class="text-zinc-500 transition-all hover:text-white"
          @click="closeMessageCard"
        >
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
      <main class="p-4">
        <div class="flex items-center justify-center text-zinc-300 gap-2">
          <h6 class="font-semibold">Ups!Sem Notificações</h6>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="16"
            height="16"
            fill="currentColor"
            class="bi bi-emoji-frown-fill w-5 h-5"
            viewBox="0 0 16 16"
          >
            <path
              d="M8 16A8 8 0 1 0 8 0a8 8 0 0 0 0 16zM7 6.5C7 7.328 6.552 8 6 8s-1-.672-1-1.5S5.448 5 6 5s1 .672 1 1.5zm-2.715 5.933a.5.5 0 0 1-.183-.683A4.498 4.498 0 0 1 8 9.5a4.5 4.5 0 0 1 3.898 2.25.5.5 0 0 1-.866.5A3.498 3.498 0 0 0 8 10.5a3.498 3.498 0 0 0-3.032 1.75.5.5 0 0 1-.683.183zM10 8c-.552 0-1-.672-1-1.5S9.448 5 10 5s1 .672 1 1.5S10.552 8 10 8z"
            />
          </svg>
        </div>
        <div class="text-center mt-5 px-1 w-full">
          <small class="font-medium text-white">
            Aqui Estarão Todas as Novidades e Atualizações Relacionadas á Escola
            de Programação 42!
          </small>
          <br />
          <div class="mt-3">
            <a
              href="https://42Luanda.com"
              class="text-center more text-cyan-300 underline"
              >Saber mais</a
            >
          </div>
        </div>
      </main>
    </div>
  </aside>
</template>
<script setup>
function closeMessageCard() {
  const messageComponent = document.querySelector(".back");
  const CardMessage = document.querySelector(".card-message");
  messageComponent.classList.add("hidden");
  CardMessage.classList.remove("showCardMessage");
  document.body.style.overflow = "auto";
}
</script>

<style scoped>
.more {
  font-size: 14px;
}
.back {
  background-color: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(12px);
}
.card-message {
  transition: transform 0.24s ease-in-out;
  transform: translateY(-60rem);
}
.showCardMessage {
  animation: showCardMessage 0.18s 0.25s ease-in-out forwards;
}
@keyframes showCardMessage {
  from {
    transform: translateY(-60rem);
    opacity: 0.5;
  }
  to {
    transform: translateY(0rem);
    opacity: 1;
  }
}
</style>
