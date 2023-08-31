<script setup>
import Accordion from "./Accordion.vue";
import TutorialCard from "./TutorialCard.vue";
</script>
<template>
  <section>
    <div class="text-center mt-10 p-5">
      <h2 class="text-zinc-200 text-4xl font-bold selection">FAQ</h2>
      <h6 class="pt-3 text-zinc-400 text-xl font-semibold">
        Tira as tuas dúvidas e prepara-te para fazeres parte da 42 Luanda!
      </h6>
    </div>
    <!-- ACCORDIONS -->
    <aside class="w-full mt-3 p-3">
      <div
        class="accordionGroup max-w-2xl w-full m-auto grid grid-cols-1 gap-4"
      >
        <Accordion
          question="O Que é a 42?"
          response=" A 42 é dos melhores centros de excelência de programação do mundo, em que
      se aprende de forma diferente assente no trabalho em equipa e em projectos
      práticos (gamificação), em vez de uma formação teórica, ganhando-se pontos
      e passando-se de nível, como se fosse um jogo. Está aberta a todos os
      interessados com idade igual ou superior a 17 anos, com ou sem diploma ou
      formação prévia em programação."
        />
        <Accordion
          question="A 42 Luanda não Cobra Propina?"
          response="Sim, desde os processos de selecção até à conclusão 
          da aprendizagem, não existem propinas, taxas ou quaisquer outras
           cobranças que possam inviabilizar o teu futuro. Não gastas um único 
           kwanza pois és patrocinado por empresas ou mecenas comprometidos com 
           o propósito de partilhar para evoluir."
        />
        <Accordion
          question="A 42 Luanda é Presencial?"
          response="Sim, o método de aprendizagem da 42 Luanda é presencial. Tens de estar em contacto directo com outros 
          estudantes, é o que chamamos de aprendizagem entre pares. Cada um contribui e, todos através da troca de conhecimentos avançam."
        />
        <Accordion
          question="É Verdade que na 42 não Tem Professores?"
          response="Sim, é verdade. Na 42 Luanda não existem professores tradicionais nem aulas expositivas. 
          Há uma plataforma online que fornece todos os desafios e projectos para os estudantes. Esta plataforma
           é transversal a toda a experiência de aprendizagem na 42 Luanda. Também existe um staff de mentores e 
           ex-alunos que podem ajudar a orientar e aconselhar os estudantes. Mas, 
          em última análise, é o teu esforço, a tua pesquisa e o trabalho com os teus colegas que te irão ajudar a superar os desafios."
        />
        <Accordion
          question="Quanto Tempo Leva para Concluir o Programa?"
          response="Se te empenhares a estudar 40 horas por semana, ao fim de 16 meses terás o Certificado Human Coder . 
          Transformar-te-ás num programador, apto a lidar de forma autónoma, criativa e colaborativa com problemas complexos.
           Ao aprofundar os estudos,
           conseguirás alcançar níveis superiores e estarás apto para abordar projectos de maior complexidade (entre 3 a 5 anos de estudo)."
        />
      </div>
    </aside>

    <!-- PROCESSO DE SELEÇÃO -->
    <h2 class="pt-8 text-zinc-200 text-center text-4xl font-bold selection">
      Processo de Seleção
    </h2>
    <div class="mt-3 max-w-5xl w-full p-5 grid grid-cols-1 m-auto">
      <TutorialCard
        tema="Inscrição Online"
        context=" A tua jornada até te tornares aprendiz na 42 Luanda começa com uma
         inscrição e candidatura pelo nosso site. "
        icon="bi bi-person-check pe-2"
      />
      <TutorialCard
        tema="Jogos de Lógica Online"
        context=" Depois de te inscreveres, e aceitares os termos e condições de participação,
         tens de saber que tens que fazer 2 jogos - online. Estes jogos foram desenhados para desafiar
          a tua capacidade de raciocínio lógico e resolução de problemas, e são o teu primeiro teste. 
          O teu desempenho será avaliado e, em até 48 horas após teres concluído, 
        receberás um e-mail com o teu resultado, indicando se avanças ou não para a fase seguinte "
        icon="bi bi-joystick pe-2"
      />
      <TutorialCard
        tema="Check-in"
        context="  Se fores aprovado nos jogos, o próximo passo é a sessão de Check-In, 
        realizada nas instalações da 42 Luanda. Esta sessão, tem dois objetivos principais: Verificar a tua identidade de forma presencial - 
        Apenas quem comparecer ao Check-in para esta verificação 
        e participar da sessão explicativa será promovido a recruta, e poderá participar da piscina. | Apresentar-te a dinâmica da Piscina, 
        fazendo-te perceber
        a importância de dares o teu máximo e familiarizar-te com as regras da 42 Luanda."
        icon="bi bi-person-bounding-box pe-2"
      />
      <TutorialCard
        tema="Piscina"
        context="Se triunfares nos jogos de lógica, completares o teu check-in e te familiarizares com as regras da 
        42 Luanda, serás convidado a participar na 'Piscina'. Trata-se de um periodo de introdução aos fundamentos de
         programação onde vais aprender noções básicas de como “ter controlo” do computador. A piscina tem duração de cerca 
         de um mês. Na Piscina, vais adquirir os teus primeiros conhecimentos em programação e trabalhar em projectos práticos.
          O objetivo é ver como te adaptas à pressão, como trabalhas em equipa e como enfrentas desafios e se tens o que é necessário
        para entregar os
         trabalhos nos prazos definidos. Não precisas de qualquer experiência prévia em programação para participar. Importante é tentar! "
        icon="bi bi-play-fill pe-2"
      />
      <TutorialCard
        tema="Admissão"
        context=" No final da Piscina, os participantes são avaliados com base na sua dedicação, progresso, 
        habilidades de trabalho em equipa e capacidade de aprender de forma autónoma. Se fores bem sucedido(a), 
        serás convidado(a) a integrar a 42 Luanda como aprendiz de programação a tempo inteiro. "
        icon="bi bi-check-all pe-2"
      />
    </div>
  </section>
</template>
<style scoped>
.selection {
  font-family: "Poppins", sans-serif;
}
</style>
