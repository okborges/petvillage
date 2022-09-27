<template>
  <header class="text-white py-3">
    <nav class="container mx-auto items-center justify-between gap-5 lg:flex">
      <img src="~/assets/Pet Village.svg" alt="logo" />
      <ul
        class="flex text-xl font-semibold items-center text-center gap-4 lg:gap-10"
      >
        <li><NuxtLink to="/#derma">Dermatologia e Alergologia</NuxtLink></li>
        <li><NuxtLink to="/#banho">Banho e tosa</NuxtLink></li>
        <li><NuxtLink to="/#hotel">Hotel</NuxtLink></li>
        <li><NuxtLink to="/#creche">Creche</NuxtLink></li>
        <li><NuxtLink to="/#cursos">Cursos</NuxtLink></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
header {
  background: #ff457e;

  li {
    padding: 6px 20px;
    cursor: pointer;
  }

  li:hover {
    background-color: #ff749e;
    border-radius: 30px;
    transition: 0.5s;
  }
}

@media screen and (max-width: 1024px) {
  header {
    img {
      margin-left: auto;
      margin-right: auto;
      margin-bottom: 10px;
    }

    ul {
      flex-wrap: wrap;
      justify-content: center;

      li {
        padding: 4px 10px;
        background-color: #ff749e;
        border-radius: 4px;
        font-size: 16px;
      }
    }
  }
}
</style>
