<template>
  <section class="w-full" id="topicos">
    <div class="text-center">
      <h2 class="text-zinc-200 text-3xl md:text-4xl font-bold">Tópicos</h2>
      <div class="w-16 rounded-md mx-auto mt-5 bg-cyan-300 h-1"></div>
    </div>

    <!-- GRID TOPICS -->
    <div
      class="w-full grid md:grid-cols-2 grid-cols-1 p-5 lg:p-3 lg:grid-cols-3 gap-4 mt-7"
    >
      <TopicBlock
        iconName="bi bi-globe-europe-africa text-cyan-300"
        tittleText="Rede Global"
        text="
        São 50 campus espalhados em 29 países, dentre elas a 42 Luanda, com mais
        de 18.000 alunos a aprender programação e a trocar experiências entre
        si.
      "
      />
      <TopicBlock
        iconName="bi bi-bar-chart text-cyan-300"
        tittleText="Formação Necessária"
        text="
        Não precisas de ter grau académico. Basta, teres mais de 17 anos e muita vontade de aprender. A tua mudança de vida passa pela 42 Luanda. 
      "
      />
      <TopicBlock
        iconName="bi bi-cart-x text-cyan-300"
        tittleText="A 0 Kwanzas"
        text="
        Não há custos antes, durante ou após a formação. É totalmente gratuita. O único valor que nos interessa é o teu valor.
      "
      />
      <TopicBlock
        iconName="bi bi-bookmarks text-cyan-300"
        tittleText="Sem Professores"
        text="
        A 42 Luanda utiliza um modelo pedagógico inovador que te permite aprender a programar por meio de desafios práticos e projectos em grupo. Não se trata de um modelo convencional por não ter professores. 
      "
      />
      <TopicBlock
        iconName="bi bi-star text-cyan-300"
        tittleText="Aprendizagem por Escala"
        text="
        Na 42 avanças no programa ganhando pontos em cada projecto que completas. Com os pontos, passas de nível e desbloqueias mais projectos no currículo da 42 em diferentes áreas da programação como, cybersegurança, inteligência artificial...
      "
      />
      <TopicBlock
        iconName="bi bi-person text-cyan-300"
        tittleText="Presencial é Essencial"
        text="
        A metodologia de ensino da 42 promove a interacção e o desenvolvimento na aprendizagem entre pares e trabalho em grupo, muito mais promissor quando feito presencialmente sendo a presença obrigatória. 
      "
      />
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

<script setup>
import TopicBlock from "./TopicBlock.vue";
</script>

<style scoped>

h2 {
  font-family: "Poppins", sans-serif;
}
</style>
