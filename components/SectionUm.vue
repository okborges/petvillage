<template>
  <section>
    <div class="container mx-auto grid lg:grid-cols-2 items-center">
      <div class="flex flex-col items-center">
        <img
          class="mb-6 rounded-lg"
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
    <div class="nav-cards container mx-auto gap-10">
      <div class="cards cor-1">
        <img src="~/assets/icons/derma.svg" alt="" />
        <p>Dermatologia e Alergologia</p>
      </div>

      <div class="cards cor-2">
        <img src="~/assets/icons/banho.svg" alt="" />
        <p>Banho e Tosa</p>
      </div>

      <div class="cards cor-3">
        <img src="~/assets/icons/hotel.svg" alt="" />
        <p>Hotel</p>
      </div>

      <div class="cards cor-4">
        <img src="~/assets/icons/creche.svg" alt="" />
        <p>Creche</p>
      </div>

      <div class="cards cor-5">
        <img src="~/assets/icons/cursos.svg" alt="" />
        <p>Cursos</p>
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
    box-shadow: 4px 6px 10px rgba(7, 21, 28, 0.2);
    border-radius: 37.3333px;
    border: 3px solid #ff457e;
  }
  button:hover {
    border: 3px solid #cc3765;
    transition: 0.2s;
  }

  .patinhas {
    background-image: url('~/assets/img/teste.svg');
    background-repeat: no-repeat;
    background-size: contain;
  }

  .nav-cards {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
  }

  .cards {
    position: relative;
    top: 4.125rem;
    display: grid;
    justify-items: center;
    text-align: center;
    align-items: center;
    background: #fff;
    padding: 0.9375rem;
    max-width: 12.4375rem;
    box-shadow: 0px 6px 10px rgba(0, 0, 0, 0.25);
    border-radius: 20px;
    cursor: pointer;

    img {
      padding-bottom: 0.3125rem;
    }
  }

  .cor-1 {
    background-color: #89e5d2;
    border: 3px solid #89e5d2;
  }
  .cor-2 {
    background-color: #ff457e;
    border: 3px solid #ff457e;
  }
  .cor-3 {
    background-color: #fed501;
    border: 3px solid #fed501;
  }
  .cor-4 {
    background-color: #ffa370;
    border: 3px solid #ffa370;
  }
  .cor-5 {
    background-color: #b38fff;
    border: 3px solid #b38fff;
  }

  .cor-1:hover {
    border: 3px solid #142721;
    transition: 0.3ss;
  }
  .cor-2:hover {
    border: 3px solid #40111f;
    transition: 0.3ss;
  }
  .cor-3:hover {
    border: 3px solid #352d00;
    transition: 0.3ss;
  }
  .cor-4:hover {
    border: 3px solid #3d271b;
    transition: 0.3ss;
  }
  .cor-5:hover {
    border: 3px solid #1b1526;
    transition: 0.3ss;
  }
}

@media screen and (max-width: 1024px) {
  section {
    .nav-cards {
      grid-template-columns: 1fr;
      .cards {
        width: inherit;
        margin-left: auto;
        margin-right: auto;
        top: 0rem;
      }
    }
  }
}
</style>
