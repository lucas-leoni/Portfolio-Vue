<template>
  <div class="row justify-content-between">
    <div class="col-4 px-4 py-4">
      <h1>{{ title() }}</h1>
    </div>
    <div class="col-7 p-0">
      <nav class="py-4">
        <ul class="list-unstyled d-flex justify-content-evenly m-0">
          <li>
            <router-link class="navbar-brand text-light" to="/">
              About
            </router-link>
          </li>
          <li>
            <router-link class="navbar-brand text-light" to="/skills">
              Skills
            </router-link>
          </li>
          <li>
            <router-link class="navbar-brand text-light" to="/portfolio">
              Portfolio
            </router-link>
          </li>
          <li>
            <router-link class="navbar-brand text-light" to="/register">
              Register
            </router-link>
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>
<script>
export default {
  name: "Navbar",
  methods: {
    title() {
      if (this.$route.name === "home") {
        return "About Me";
      }
      if (this.$route.name === "Skills") {
        return "Skills";
      }
      if (this.$route.name === "Portfolio") {
        return "Portfolio";
      }
      if (this.$route.name === "Register") {
        return "Register";
      }
    },
  },
};
</script>
<style scoped>
nav {
  border: 1px solid hsl(0, 0%, 22%);
  background-color: #282829;
  border-bottom-left-radius: 1rem;
  border-top-right-radius: 1rem;
}
</style>
