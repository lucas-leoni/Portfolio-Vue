<template>
  <div>
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
    <div v-if="rotaSkills" class="container">
      <div class="row">
        <div class="col py-5">
          <h2>Database</h2>
          <div id="skills" class="p-3 mt-4 mb-5">
            <h5>MySQL - 65%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 65%"></div>
            </div>
            <h5>SQL Server - 60%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 60%"></div>
            </div>
            <h5>MongoDB - 50%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="w-50 rounded-pill" id="skill"></div>
            </div>
          </div>
          <h2 class="pt-4">Backend</h2>
          <div id="skills" class="p-3 my-4">
            <h5>Python - 65%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 65%"></div>
            </div>
            <h5>JavaScript em Node.js - 65%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 65%"></div>
            </div>
          </div>
        </div>
        <div class="col py-5">
          <h2>Frontend</h2>
          <div id="skills" class="p-3 mt-4 mb-5">
            <h5>HTML - 60%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 60%"></div>
            </div>
            <h5>CSS - 65%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 65%"></div>
            </div>
            <h5>JavaScript - 65%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 65%"></div>
            </div>
          </div>
          <h2 class="pt-4">Versionamento</h2>
          <div id="skills" class="p-3 my-4">
            <h5>Git - 60%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 60%"></div>
            </div>
            <h5>GitHub - 60%</h5>
            <div class="w-100 rounded-pill my-3" id="bg-skill">
              <div class="rounded-pill" id="skill" style="width: 60%"></div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div v-if="rotaPortfolio" class="container py-5 my-3">
      <div class="row justify-content-evenly">
        <div class="col-5">
          <img src="../assets/project1.jpg" width="260" height="200" />
          <h6 class="mt-3">Finance</h6>
          <p class="mb-5">Web development</p>
        </div>
        <div class="col-5">
          <img src="../assets/project2.png" width="260" height="200" />
          <h6 class="mt-3">Orizon</h6>
          <p class="mb-5">Web development</p>
        </div>
      </div>
      <div class="row justify-content-evenly">
        <div class="col-5">
          <img src="../assets/project3.jpg" width="260" height="200" />
          <h6 class="mt-3">Fundo</h6>
          <p class="m-0">Web design</p>
        </div>
        <div class="col-5">
          <img src="../assets/project4.png" width="260" height="200" />
          <h6 class="mt-3">Brawlhalla</h6>
          <p class="m-0">Applications</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Main",
  computed: {
    rotaAbout() {
      return this.$route.name === "home";
    },
    rotaSkills() {
      return this.$route.name === "Skills";
    },
    rotaPortfolio() {
      return this.$route.name === "Portfolio";
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
#skills {
  border: 1px solid hsl(0, 0%, 22%);
  border-radius: 1rem;
}
#bg-skill {
  background-color: #383838;
  height: 1rem;
}
#skill {
  background-color: #1bc4a7;
  height: 1rem;
}
img {
  border-radius: 1rem;
}
</style>
