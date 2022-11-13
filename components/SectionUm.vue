<template>
  <section class="pb-10 lg:pb-0">
    <div class="container mx-auto grid lg:grid-cols-2 items-center">
      <div class="flex flex-col items-center">
        <div class="flic">
          <Flicking
            :options="{
              circular: true,
            }"
            :plugins="plugins"
          >
            <img
              class="rounded-lg"
              src="~/assets/img/logo_novo.webp"
              alt="logotipo"
            />
            <img
              class="rounded-lg"
              src="~/assets/img/faixada.webp"
              alt="logotipo"
            />
            <img
              class="rounded-lg"
              src="~/assets/img/faixada_2.webp"
              alt="logotipo"
            />
          </Flicking>
        </div>

        <button class="text-white text-2xl font-semibold">
          <a href="https://wa.me/5511981287333" target="_blank"
            >ENTRAR EM CONTATO</a
          >
        </button>
      </div>

      <div>
        <img
          src="~/assets/img/2main.webp"
          alt="foto capa"
          width="765"
          height="641"
        />
      </div>
    </div>

    <div class="nav-cards container mx-auto gap-10">
      <NuxtLink to="#derma" class="cards cor-1">
        <img src="~/assets/icons/derma.svg" alt="dermatologista" />
        <p>Dermatologia e Alergologia</p>
      </NuxtLink>

      <NuxtLink to="/#banho" class="cards cor-2">
        <img
          src="~/assets/icons/banho.svg"
          alt="banho e tosa"
          width="50"
          height="55"
        />
        <p>Banho e Tosa</p>
      </NuxtLink>

      <NuxtLink to="/#hotel" class="cards cor-3">
        <img
          src="~/assets/icons/hotel.svg"
          alt="hotel"
          width="53"
          height="55"
        />
        <p>Hotel</p>
      </NuxtLink>

      <NuxtLink to="/#creche" class="cards cor-4">
        <img
          src="~/assets/icons/creche.svg"
          alt="creche"
          width="52"
          height="57"
        />
        <p>Creche</p>
      </NuxtLink>

      <NuxtLink to="/#cursos" class="cards cor-5">
        <img src="~/assets/icons/cursos.svg" alt="cursos" />
        <p>Cursos</p>
      </NuxtLink>
    </div>
  </section>
</template>

<script>
import { Flicking } from '@egjs/vue-flicking';
import { AutoPlay } from '@egjs/flicking-plugins';
export default {
  components: {
    Flicking,
  },
  data: () => {
    return {
      plugins: [
        new AutoPlay({ duration: 5000, direction: 'NEXT', stopOnHover: false }),
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
section {
  background-color: #3dbeff;

  .flic {
    max-width: 28.75rem;
    margin-bottom: 1.25rem;
    img {
      width: 28.75rem;
      height: 25rem;
    }
  }

  p {
    font-size: 1.5rem;
    font-weight: 600;
  }

  button {
    padding: 1.25rem 1.875rem;
    background: #ff457e;
    box-shadow: 0.25rem 0.375rem 0.625rem rgba(7, 21, 28, 0.2);
    border-radius: 2.3333rem;
    border: 0.1875rem solid #ff457e;
    transition: 0.3s;
  }
  button:hover {
    border: 0.1875rem solid #cc3765;
    transform: scale(1.02);
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
    box-shadow: 0rem 0.375rem 0.625rem rgba(0, 0, 0, 0.25);
    border-radius: 1.25rem;
    cursor: pointer;
    transition: 0.3s;

    img {
      padding-bottom: 0.3125rem;
    }
  }

  .cor-1 {
    color: #142721;
    background-color: #89e5d2;
    border: 0.1875rem solid #89e5d2;
    transition: 0.3s;
  }
  .cor-2 {
    color: #40111f;
    background-color: #ff457e;
    border: 0.1875rem solid #ff457e;
    transition: 0.3s;
  }
  .cor-3 {
    color: #352d00;
    background-color: #fed501;
    border: 0.1875rem solid #fed501;
    transition: 0.3s;
  }
  .cor-4 {
    color: #3d271b;
    background-color: #ffa370;
    border: 0.1875rem solid #ffa370;
    transition: 0.3s;
  }
  .cor-5 {
    color: #1b1526;
    background-color: #b38fff;
    border: 0.1875rem solid #b38fff;
    transition: 0.3s;
  }

  .cor-1:hover {
    border: 0.1875rem solid #142721;
    transform: scale(1.02);
  }
  .cor-2:hover {
    border: 0.1875rem solid #40111f;
    transform: scale(1.02);
  }
  .cor-3:hover {
    border: 0.1875rem solid #352d00;
    transform: scale(1.02);
  }
  .cor-4:hover {
    border: 0.1875rem solid #3d271b;
    transform: scale(1.02);
  }
  .cor-5:hover {
    border: 0.1875rem solid #1b1526;
    transform: scale(1.02);
  }
}

@media screen and (max-width: 64rem) {
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
