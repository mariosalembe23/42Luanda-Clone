<template>
  <header class="w-full h-screen header relative" id="sobre">
    <div class="mask">
      <div
        class="navbar z-20 transition-all fixed top-0 left-0 right-0 w-full h-16 p-3 md:p-5 flex items-center justify-between lg:justify-around"
      >
        <div>
          <a href="#" class="logo text-white font-semibold text-xl"
            >42 | Luanda</a
          >
        </div>
        <div>
          <nav>
            <ul class="flex items-center space-x-4">
              <li>
                <a
                  href="#topicos"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Sobre</a
                >
              </li>
              <li>
                <a
                  href="#vantagens"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Vantagens</a
                >
              </li>
              <li>
                <a
                  href="#comunidade"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Comunidade</a
                >
              </li>
              <li>
                <a
                  href="#FAQ"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >FAQ</a
                >
              </li>
              <li>
                <div
                  class="px-4 md:border-l border-white border-opacity-60 flex items-center space-x-3 md:space-x-4"
                >
                  <a
                    href="#"
                    class="text-cyan-100 transition-all hover:text-cyan-300"
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
                        d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
                      />
                    </svg>
                  </a>
                  <a
                    href="#"
                    class="text-cyan-100 md:inline-block hidden transition-all hover:text-cyan-300"
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
                  </a>
                  <a
                    href="#"
                    class="text-cyan-100 md:inline-block hidden transition-all hover:text-cyan-300"
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
                        d="M7.5 8.25h9m-9 3H12m-9.75 1.51c0 1.6 1.123 2.994 2.707 3.227 1.129.166 2.27.293 3.423.379.35.026.67.21.865.501L12 21l2.755-4.133a1.14 1.14 0 01.865-.501 48.172 48.172 0 003.423-.379c1.584-.233 2.707-1.626 2.707-3.228V6.741c0-1.602-1.123-2.995-2.707-3.228A48.394 48.394 0 0012 3c-2.392 0-4.744.175-7.043.513C3.373 3.746 2.25 5.14 2.25 6.741v6.018z"
                      />
                    </svg>
                  </a>
                  <button
                    @click="OpenOffCanvas"
                    class="text-cyan-100 inline-block md:hidden transition-all hover:text-cyan-300"
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
                        d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
                      />
                    </svg>
                  </button>
                </div>
              </li>
            </ul>
          </nav>
        </div>
      </div>
      <!-- BANNER -->
      <section class="w-full h-full flex items-center justify-center">
        <div class="banner max-w-5xl w-full m-auto text-center p-3">
          <h1
            class="text-cyan-100 text-4xl md:text-4xl lg:text-6xl font-extrabold principalText"
          >
            Aprenda a Programar do Zero
          </h1>

          <div class="textIntroduce mx-auto mt-3">
            <p class="font-medium text-white text-xl">
              Esta é a tua porta para o futuro! Torna-te um profissional de
              programação disputado pelas melhores empresas.
            </p>
          </div>
          <div
            class="flex lg:flex-row flex-col items-center justify-center mt-5 gap-3"
          >
            <a
              href="#"
              class="bg-cyan-300 w-full md:w-40 rounded-md flex items-center justify-center py-3 px-3 text-zinc-950 font-semibold transition-all hover:bg-cyan-200"
              >Entrar
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5 ms-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M15.75 6a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0zM4.501 20.118a7.5 7.5 0 0114.998 0A17.933 17.933 0 0112 21.75c-2.676 0-5.216-.584-7.499-1.632z"
                /></svg
            ></a>
            <a
              href="#FAQ"
              class="bg-zinc-950 w-full md:w-40 rounded-md flex items-center justify-center py-3 px-3 text-cyan-300 font-semibold transition-all hover:bg-zinc-900"
              >FAQ
              <svg
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="currentColor"
                class="w-5 h-5 ms-1"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M9.879 7.519c1.171-1.025 3.071-1.025 4.242 0 1.172 1.025 1.172 2.687 0 3.712-.203.179-.43.326-.67.442-.745.361-1.45.999-1.45 1.827v.75M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-9 5.25h.008v.008H12v-.008z"
                />
              </svg>
            </a>
          </div>
        </div>
      </section>
    </div>
    <!-- ICON FLUTUANT -->

    <svg
      xmlns="http://www.w3.org/2000/svg"
      fill="none"
      viewBox="0 0 24 24"
      stroke-width="1.5"
      stroke="currentColor"
      class="w-8 h-8 absolute iconFloat text-white"
    >
      <path
        stroke-linecap="round"
        stroke-linejoin="round"
        d="M19.5 5.25l-7.5 7.5-7.5-7.5m15 6l-7.5 7.5-7.5-7.5"
      />
    </svg>
  </header>

  <offcanvas />
</template>

<script setup>
import Offcanvas from "./Offcanvas.vue";
window.addEventListener("load", () => {
  const navbar = document.querySelector(".navbar");

  if (!navbar) {
    return;
  }

  const scrollNavbarAction = () => {
    if (window.scrollY === 0) {
      navbar.classList.remove("navbarScroll");
    } else {
      navbar.classList.add("navbarScroll");
    }
  };

  scrollNavbarAction();

  document.addEventListener("scroll", scrollNavbarAction);
});
function OpenOffCanvas() {
  const offCanvas = document.querySelector(".offcanvas");

  offCanvas.classList.add("showOffCanvas");
  document.body.style.overflow = "hidden";
}
</script>

<style scoped>
.iconFloat {
  font-size: 2.4rem;
  transform: translate(-50%, -50%);
  left: 50%;
  transition: all 1s ease-in-out;
  animation: float 1s ease-in-out alternate infinite;
}
@keyframes float {
  from {
    bottom: 2rem;
  }
  to {
    bottom: 0rem;
  }
}
.navbarScroll {
  backdrop-filter: blur(10px);
  background-color: rgba(0, 0, 0, 0.5);
}
.header {
  background-image: url("/images/fundo.jpg");
  background-size: cover;
  background-position: top center;
}
.mask {
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}
.navbarLink {
  font-size: 15px;
  font-family: "Poppins", sans-serif;
}
.logo {
  font-family: "Poppins", sans-serif;
}
i {
  font-size: 1.2rem;
}
.principalText {
  font-family: "Poppins";
}
.textIntroduce {
  max-width: 40rem;
  width: 100%;
}
.card {
  max-width: 30rem;
  width: 100%;
  background-color: rgba(0, 0, 0, 0.1);
}
</style>
