<template>
  <div id="app">
    <div class="container p-5">
      <div class="row justify-content-evenly">
        <div id="aside" class="col-3">
          <Aside />
        </div>
        <div id="main" class="col-8">
          <main class="text-light">
            <Navbar />
            <router-view />
          </main>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Aside from "@/components/Aside.vue";
import Navbar from "@/components/Navbar.vue";

export default {
  name: "App",
  components: {
    Aside,
    Navbar,
  },
};
</script>
<style scoped>
#app {
  background-color: hsl(0, 0%, 7%);
}
#aside {
  border: 1px solid hsl(0, 0%, 22%);
  background-color: hsl(240, 2%, 12%);
  border-radius: 1rem;
  height: 80vh;
}
#main {
  border: 1px solid hsl(0, 0%, 22%);
  background-color: hsl(240, 2%, 12%);
  border-radius: 1rem;
  height: 89.8vh;
}
</style>
