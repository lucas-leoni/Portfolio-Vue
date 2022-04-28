<template>
  <aside class="p-4 text-light d-flex flex-column align-content-center">
    <img
      class="align-self-center mt-4"
      src="../assets/image.webp"
      width="150"
      height="200"
    />
    <h3 class="text-center mt-4">{{ nomeCompleto }}</h3>
    <hr />
    <ul class="list-unstyled">
      <li class="py-3">
        <div class="row">
          <div class="col-2 p-0 d-flex justify-content-end">
            <i class="bi bi-envelope"></i>
          </div>
          <div class="col-10">
            <p class="m-0">EMAIL</p>
            <p class="m-0">
              <a class="text-decoration-none text-light" v-bind:href="email">
                {{ this.aside.email }}
              </a>
            </p>
          </div>
        </div>
      </li>
      <li class="py-3">
        <div class="row">
          <div class="col-2 p-0 d-flex justify-content-end">
            <i class="bi bi-phone"></i>
          </div>
          <div class="col-10">
            <p class="m-0">PHONE</p>
            <p class="m-0">
              <a class="text-decoration-none text-light" v-bind:href="phone">
                {{ this.aside.phone }}
              </a>
            </p>
          </div>
        </div>
      </li>
      <li class="py-3">
        <div class="row">
          <div class="col-2 p-0 d-flex justify-content-end">
            <i class="bi bi-calendar3"></i>
          </div>
          <div class="col-10">
            <p class="m-0">BIRTHDAY</p>
            <p class="m-0">
              <a class="text-decoration-none text-light">
                {{ this.aside.birthday }}
              </a>
            </p>
          </div>
        </div>
      </li>
      <li class="py-3">
        <div class="row">
          <div class="col-2 p-0 d-flex justify-content-end">
            <i class="bi bi-geo-alt"></i>
          </div>
          <div class="col-10">
            <p class="m-0">LOCATION</p>
            <p class="m-0">
              <a class="text-decoration-none text-light">
                {{ this.aside.location }}
              </a>
            </p>
          </div>
        </div>
      </li>
      <li class="py-3 d-flex justify-content-evenly">
        <a
          class="text-decoration-none text-light"
          v-bind:href="this.aside.linkedin"
        >
          <i id="icone_menor" class="bi bi-linkedin"></i>
        </a>
        <a
          class="text-decoration-none text-light"
          v-bind:href="this.aside.github"
        >
          <i id="icone_menor" class="bi bi-github"></i>
        </a>
        <a
          class="text-decoration-none text-light"
          v-bind:href="this.aside.whatsapp"
        >
          <i id="icone_menor" class="bi bi-whatsapp"></i>
        </a>
      </li>
    </ul>
  </aside>
</template>
<script>
export default {
  name: "Aside",
  data() {
    return {
      aside: {
        name: "Lucas",
        lastname: "Leoni",
        email: "lucas.leoni09@gmail.com",
        phone: "+55 (47) 99701-1007",
        birthday: "May 4, 2000",
        location: "Joinville, Santa Catarina, BR",
        linkedin: "https://www.linkedin.com/in/lucas-leoni09",
        github: "https://github.com/lucas-leoni",
        whatsapp:
          "https://api.whatsapp.com/send?phone=5547997011007&text=Ol%C3%A1,%20Lucas",
      },
    };
  },
  computed: {
    nomeCompleto() {
      return this.aside.name + " " + this.aside.lastname;
    },
    email() {
      return "mailto:" + this.aside.email;
    },
    phone() {
      return "tel:" + this.aside.phone;
    },
  },
};
</script>
<style scoped>
i {
  font-size: 2rem;
}
#icone_menor {
  font-size: 1.25rem;
}
img {
  border-radius: 1rem;
}
</style>
