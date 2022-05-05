<template>
  <div v-if="rotaPortfolio" class="container py-5 my-3">
    <div class="row justify-content-evenly">
      <div class="col-5">
        <img src="../../assets/project1.jpg" width="260" height="200" />
        <h6 class="mt-3">Finance</h6>
        <p class="mb-5">Web development</p>
      </div>
      <div class="col-5">
        <img src="../../assets/project2.png" width="260" height="200" />
        <h6 class="mt-3">Orizon</h6>
        <p class="mb-5">Web development</p>
      </div>
    </div>
    <div class="row justify-content-evenly">
      <div class="col-5">
        <img src="../../assets/project3.jpg" width="260" height="200" />
        <h6 class="mt-3">Fundo</h6>
        <p class="m-0">Web design</p>
      </div>
      <div class="col-5">
        <img src="../../assets/project4.png" width="260" height="200" />
        <h6 class="mt-3">Brawlhalla</h6>
        <p class="m-0">Applications</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "PortfolioMain",
  computed: {
    rotaPortfolio() {
      return this.$route.name === "Portfolio";
    },
  },
};
</script>
<style scoped>
img {
  border-radius: 1rem;
}
</style>
