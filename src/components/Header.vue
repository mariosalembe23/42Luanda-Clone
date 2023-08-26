<template>
  <header class="w-full h-screen header relative">
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
                  href="#"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Sobre</a
                >
              </li>
              <li>
                <a
                  href="#"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Vantagens</a
                >
              </li>
              <li>
                <a
                  href="#"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Comunidade</a
                >
              </li>
              <li>
                <a
                  href="#"
                  class="navbarLink md:inline-block hidden font-medium text-white transition-all hover:text-cyan-200"
                  >Ajuda</a
                >
              </li>
              <li>
                <div
                  class="px-4 md:border-l border-white border-opacity-60 flex items-center space-x-3 md:space-x-5"
                >
                  <a
                    href="#"
                    class="text-cyan-100 transition-all hover:text-cyan-300"
                  >
                    <i class="bi bi-door-open"></i>
                  </a>
                  <a
                    href="#"
                    class="text-cyan-100 md:inline-block hidden transition-all hover:text-cyan-300"
                  >
                    <i class="bi bi-bell"></i>
                  </a>
                  <a
                    href="#"
                    class="text-cyan-100 md:inline-block hidden transition-all hover:text-cyan-300"
                  >
                    <i class="bi bi-instagram"></i>
                  </a>
                  <a
                    href="#"
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
                  </a>
                </div>
              </li>
            </ul>
          </nav>
        </div>
      </div>
      <!-- BANNER -->
      <section class="w-full h-full flex items-center justify-center">
        <div class="banner max-w-5xl w-full m-auto text-center p-5">
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
            class="flex md:flex-row flex-col items-center justify-center mt-5 gap-3"
          >
            <a
              href="#"
              class="bg-cyan-300 w-full md:w-40 rounded-md flex items-center justify-center py-3 px-3 text-zinc-950 font-semibold transition-all hover:bg-cyan-200"
              >Entrar <i class="bi bi-door-open ms-1"></i
            ></a>
            <a
              href="#"
              class="bg-zinc-950 w-full md:w-40 rounded-md flex items-center justify-center py-3 px-3 text-cyan-300 font-semibold transition-all hover:bg-zinc-900"
              >FAQ <i class="bi bi-question-circle ps-1"></i
            ></a>
          </div>
        </div>
      </section>
    </div>
    <!-- ICON FLUTUANT -->
    <i class="bi bi-chevron-double-down text-white absolute iconFloat"> </i>
  </header>
</template>

<script setup>
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

  scrollNavbarAction()

  document.addEventListener("scroll", scrollNavbarAction)
});
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
  background-color: rgba(0, 0, 0, 0.2);
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
