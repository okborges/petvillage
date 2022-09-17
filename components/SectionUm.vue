<template>
  <section>
    <div class="container mx-auto grid lg:grid-cols-2">
      <div>
        <img
          src="~/assets/img/logo.jpg"
          alt="logotipo"
          width="460"
          height="306"
        />
        <button class="text-white text-2xl font-semibold">
          <a href="">ENTRAR EM CONTATO</a>
        </button>
      </div>

      <div class="patinhas">
        <img src="~/assets/img/dogs-inicial.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
section {
  background-color: #3dbeff;

  button {
    padding: 20px 30px;
    background: #ff457e;
    border: 3px solid #cc3765;
    box-shadow: 4px 6px 10px rgba(7, 21, 28, 0.2);
    border-radius: 37.3333px;
  }

  .patinhas {
    background-image: url('~/assets/img/teste.svg');
    background-repeat: no-repeat;
    background-size: contain;
  }
}
</style>
