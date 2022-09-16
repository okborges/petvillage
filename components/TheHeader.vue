<template>
  <header class="text-white py-3">
    <div class="container mx-auto flex items-center justify-between">
      <img src="~/assets/Pet Village.svg" alt="logo" />
      <ul class="flex gap-10 text-xl font-semibold">
        <li>Dermatologia e Alergologia</li>
        <li>Banho e tosa</li>
        <li>Hotel</li>
        <li>Creche</li>
        <li>Cursos</li>
      </ul>
    </div>
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
</style>
