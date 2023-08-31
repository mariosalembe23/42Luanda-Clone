<script></script>

<template>
  <section class="w-full" id="comunidade">
    <h2 class="text-center text-zinc-200 text-3xl md:text-4xl font-bold">
      Junte-se á Comunidade!
    </h2>
    <div class="w-16 rounded-md mx-auto mt-5 bg-cyan-300 h-1"></div>
    <div
      class="max-w-5xl w-full grid grid-cols-1 md:grid-cols-2 mt-5 m-auto gap-3 p-3"
    >
      <div class="bg-zinc-300 p-5 rounded-md">
        <header class="w-full flex items-center gap-3">
          <img
            src="/images/user1.png"
            class="w-20 h-20 rounded-full ring-4 ring-cyan-300"
            alt="imagem de Usuáio "
          />
          <div>
            <h6 class="font-semibold text-zinc-800">Jonas Simão</h6>
            <small class="text-gray-600">Participante</small>
          </div>
        </header>
        <main>
          <p class="px-3 pt-4 textComment text-zinc-900 pb-2">
            Eu quero aprender programação para desenvolver as minhas habilidades
            e capacidade de análise, para obter novas oportunidades de carreira
            e maior autonomia para criar os meus próprios projectos.
          </p>
        </main>
      </div>

      <div class="bg-zinc-300 p-5 rounded-md">
        <header class="w-full flex items-center gap-3">
          <img
            src="/images/user2.png"
            class="w-20 h-20 rounded-full ring-4 ring-cyan-300"
            alt="imagem de Usuáio "
          />
          <div>
            <h6 class="font-semibold text-zinc-800">Márcia Kiteque</h6>
            <small class="text-gray-600">Participante</small>
          </div>
        </header>
        <main>
          <p class="px-3 pt-4 textComment text-zinc-900 pb-2">
            Fiz o enter na 42 Luanda porque acredito que todos podemos ser
            protagonizadores da nossa carreira e sucesso. O futuro está nas
            nossas mãos, adquirir novas habilidades que vão impulsionar o meu
            crescimento. O conhecimento é a chave para abrir todas as portas,
            vamos juntos nessa jornada.
          </p>
        </main>
      </div>
    </div>
    <div
      class="border border-zinc-800 rounded-full text-zinc-400 text-center py-1 w-80 mt-6 m-auto flex items-center gap-1 justify-center hover:border-white hover:text-white transition-all"
    >
      <a href="#" class="sug">Ainda Podes ver mais Depoimentos &rarr;</a>
    </div>
    <div class="text-center py-4 md:py-8">
      <p class="text-cyan-400 font-semibold pb-4">Deseja Participar?</p>
      <a
        href="#"
        class="text-zinc-950 bg-cyan-400 block w-40 m-auto font-semibold rounded-md transition-all hover:ring-4 hover:ring-cyan-400 hover:ring-opacity-30  py-2.5"
        >Cadastre-se</a
      >
    </div>
  </section>
</template>

<style scoped>
h2 {
  font-family: "Poppins", sans-serif;
}
.textComment {
  font-size: 15px;
}
.sug {
  font-size: 15px;
}
</style>
