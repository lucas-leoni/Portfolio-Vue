<template>
  <div>
    <div class="row justify-content-between py-4">
      <div class="col-5">
        <div class="row">
          <label for="titulo"
            ><b>Título</b>
            <input
              type="text"
              class="form-control"
              v-model="titulo"
              placeholder="Insira um título"
            />
          </label>
        </div>
      </div>
      <div class="col-5">
        <div class="row">
          <label for="conclusao"
            ><b>Conclusão</b>
            <input type="date" class="form-control" v-model="conclusao" />
          </label>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col">
        <div class="row">
          <label for="instituicao"
            ><b>Instituição</b>
            <input
              type="text"
              class="form-control"
              v-model="instituicao"
              placeholder="Insira o nome da Instituição"
            />
          </label>
        </div>
      </div>
    </div>
    <div class="row pt-4 justify-content-between">
      <div class="col-5">
        <button @click="cancelar" type="button" class="btn btn-secondary">
          Cancelar
        </button>
      </div>
      <div class="col-5 d-flex justify-content-end">
        <button type="button" class="btn btn-primary">Salvar</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "EducationForm",
  data() {
    return {
      titulo: "",
      conclusao: "",
      instituicao: "",
    };
  },
  methods: {
    cancelar() {
      this.titulo = "";
      this.conclusao = "";
      this.instituicao = "";
    },
  },
};
</script>
