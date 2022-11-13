<template>
  <header class="text-white py-3">
    <nav class="container mx-auto items-center justify-between gap-5 lg:flex">
      <img
        src="~/assets/icons/Pet Village.svg"
        alt="logo"
        width="255"
        height="65"
      />
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
    padding: 0.375rem 1.25rem;
    cursor: pointer;
    a {
      color: #57001b;
    }
  }

  li:hover {
    background-color: #ff749e;
    border-radius: 1.875rem;
    transition: 0.5s;
  }
}

@media screen and (max-width: 64rem) {
  header {
    img {
      margin-left: auto;
      margin-right: auto;
      margin-bottom: 0.625rem;
    }

    ul {
      flex-wrap: wrap;
      justify-content: center;

      li {
        padding: 0.25rem 0.625rem;
        background-color: #ff749e;
        border-radius: 0.25rem;
        font-size: 1rem;
      }
    }
  }
}
</style>
