<template>
  <div class="container">
    <div class="col">
      <div class="row py-4">
        <h2>Adicionar Educação</h2>
        <EducationForm />
      </div>
      <hr />
      <div class="row py-4">
        <h2>Adicionar Trabalho</h2>
        <JobsForm />
      </div>
    </div>
  </div>
</template>
<script>
import EducationForm from "@/components/form/EducationForm.vue";
import JobsForm from "@/components/form/JobsForm.vue";

export default {
  name: "RegisterMain",
  components: {
    EducationForm,
    JobsForm,
  },
};
</script>
