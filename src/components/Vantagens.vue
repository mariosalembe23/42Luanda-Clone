<script setup>
import VantagensCard from "./VantagensCard.vue";
</script>

<template>
  <section class="w-full">
    <div class="text-center mt-8">
      <h2 class="text-zinc-200 text-4xl font-bold">Vantagens</h2>
      <div class="w-16 rounded-md mx-auto mt-5 bg-cyan-300 h-1"></div>
      <!-- <p>Quem faz Enter, Faz Certo!</p> -->
    </div>
    <div class="max-w-5xl m-auto w-full grid-cols-2 pb-32 grid gap-4 mt-12">
      <VantagensCard
        iconName="bi bi-alarm iconVantagem text-white"
        tittle="Sem Horários, no seu Tempo!"
        text=" Aberta 24h por dia, 7 dias por semana, permite definires o teu ritmo e
          o teu percurso, consoante a tua disponibilidade e os teus interesses."
      />
      <VantagensCard
        iconName="bi bi-people iconVantagem text-white"
        tittle="Aprendes a aprender!"
        text=" Método presencial que abrange linguagens fundamentais de programação, começando com C. Com uma base sólida e profunda."
      />
      <VantagensCard
        iconName="bi bi-code-square iconVantagem text-white"
        tittle="Aprendizagem divertida!"
        text="Na 42 Luanda, vais desenvolver habilidades de resolução de problemas, com criatividade, determinação e trabalho em equipa."
      />
      <VantagensCard
        iconName="bi bi-code-square iconVantagem text-white"
        tittle="Oportunidades sem Medida!"
        text="A partir de 18 meses de formação, os alunos podem participar em projectos de programação em empresas parceiras da 42 Luanda."
      />
      <VantagensCard
        iconName="bi bi-award iconVantagem text-white"
        tittle="Desperta o Génio em Ti!"
        text="Depois de obteres o certificado, podes entrar em diversas áreas. Inteligência Artificial, Cybersegurança, Desenvolvimento de Games..."
      />
      <a href="#" class="transition-all hover:opacity-90">
        <div
          class="bg-zinc-900 p-5 rounded-md h-44 ring-2 ring-indigo-400 grid grid-cols-6"
        >
          <div
            class="col-span-2 bg-indigo-600 rounded-md flex items-center justify-center"
          >
            <i class="bi bi-app-indicator iconMain text-indigo-100"></i>
          </div>
          <div class="col-span-4 px-3 py-2">
            <h4 class="text-indigo-300 font-semibold">
              Faça Parte Agora mesmo!
            </h4>
            <p class="textInfo pt-1 text-white pb-3">
              Não perca a oportunidade! Inscreva-se agora para fazer parte da
              nossa comunidade. Seja parte de algo incrível!
            </p>
            <small class="text-indigo-200">Clique para Participar</small>
          </div>
        </div>
      </a>
    </div>
  </section>
</template>

<style scoped>
.iconMain {
  font-size: 2.5rem;
}
.textInfo {
  font-size: 14px;
}
.link {
  font-size: 14px;
}
</style>
