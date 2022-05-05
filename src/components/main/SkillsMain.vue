<template>
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
</template>
<script>
export default {
  name: "SkillsMain",
  computed: {
    rotaSkills() {
      return this.$route.name === "Skills";
    },
  },
};
</script>
<style scoped>
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
</style>
