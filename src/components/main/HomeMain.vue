<template>
  <div v-if="rotaAbout" class="container py-4">
    <p id="about_me" class="py-3 m-0">
      Acadêmico da 5ª fase do curso de Sistemas para Internet da Faculdade
      IELUSC, tenho 21 anos e almejo meu primeiro emprego na área.
    </p>
    <p id="about_me" class="py-3 m-0">
      Com a primeira oportunidade no mercado de trabalho, busco conquistar
      experiência e colocar em prática os aprendizados da graduação.
    </p>
    <h1 class="py-4 m-0">
      <i class="bi bi-book"></i>
      Education
    </h1>
    <ul>
      <li class="py-4">
        <h5>Tecnólogo em Sistemas para Internet</h5>
        <p class="m-0">Faculdade IELUSC - Joinville, SC</p>
        <p class="m-0">Conclusão Prevista: 2022</p>
      </li>
      <li class="py-4">
        <h5>Ensino Médio</h5>
        <p class="m-0">E.E.B. Presidente Médici - Joinville, SC</p>
        <p class="m-0">Conclusão: 2017</p>
      </li>
      <li class="py-4">
        <h5>Ensino Fundamental</h5>
        <p class="m-0">E.M. Profª Maria Regina Leal - Joinville, SC</p>
        <p class="m-0">Conclusão: 2014</p>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: "HomeMain",
  computed: {
    rotaAbout() {
      return this.$route.name === "home";
    },
  },
};
</script>
<style scoped>
#about_me {
  font-size: 1.3rem;
}
i {
  font-size: 2rem;
}
</style>
