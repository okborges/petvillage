<template>
  <section id="creche">
    <div class="container mx-auto px-6 grid lg:grid-cols-2 items-center">
      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">Creche</h1>
        <p class="mb-0 lg:mb-14">
          As atividades são dirigidas para a socialização com outros Pets,
          liberdade para brincar e correr, saúde mental, alimentação e cuidados,
          conforme estão acostumados em casa, sempre respeitando a
          individualidade e natureza de cada um. Visite-nos ! <br />
          <br />
          A partir de R$40,00 / dia <br />
          Valores especiais para pacotes.
        </p>
      </div>

      <div class="verde pt-16 grid justify-center">
        <div class="flic">
          <Flicking
            :options="{
              circular: true,
            }"
            :plugins="plugins"
          >
            <img src="~/assets/img/creche.webp" alt="Fotos creche 1" />
            <img src="~/assets/img/creche4.webp" alt="Fotos creche 2" />
            <img src="~/assets/img/creche1.webp" alt="Fotos creche 3" />
            <img src="~/assets/img/creche3.webp" alt="Fotos creche 4" />
            <img src="~/assets/img/creche6.webp" alt="Fotos creche 5" />
          </Flicking>
        </div>
        <p class="text-center py-10 px-2">
          Contamos com um espaço amplo e arejado, com instalações ao ar livre e
          áreas cobertas, localização privilegiada, segurança, higiene e limpeza
          visando o bem-estar de todos.
        </p>
        <button class="justify-self-center mb-6">
          <a href="https://wa.me/5511981287333" target="_blank"
            >Marcar Creche</a
          >
        </button>
      </div>
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
  .flic {
    max-width: 33.375rem;
    max-height: 20.875rem;
    img {
      width: 33.375rem;
      height: 20.875rem;
      object-fit: cover;
      border-radius: 0.5rem;
    }
  }
  .verde {
    background-color: #ffa370;
    button {
      padding: 0.875rem 1.5rem;
      background: #3d271b;
      border: 0.25rem solid #3d271b;
      box-shadow: 0.1875rem 0.25rem 0.6875rem rgba(0, 0, 0, 0.4);
      border-radius: 2.5rem;
      font-size: 1.25rem;
      font-weight: 700;
      color: #ffffff;
      width: max-content;
      height: fit-content;
      transition: 0.2s;
    }
    button:hover {
      border: 0.25rem solid #a95b2f;
      transform: scale(1.02);
    }
    p {
      font-family: 'Barlow';
      font-weight: 600;
      font-size: 1.25rem;
      line-height: 1.875rem;
      color: #452310;
      max-width: 26.875rem;
      justify-self: center;
    }
  }

  .direita {
    max-width: 33.125rem;
    h1 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 2.25rem;
      line-height: 3.375rem;
      color: #3d271b;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 1.25rem;
      line-height: 1.6875rem;
      color: #814321;
      max-width: 25.625rem;
    }

    .tratamentos {
      h2 {
        font-family: 'Fraunces';
        font-weight: 700;
        font-size: 1.25rem;
        line-height: 1.75rem;
        color: #40111f;
      }
      ul {
        list-style: inside;
        li {
          font-family: 'Barlow';
          font-weight: 500;
          font-size: 0.875rem;
          line-height: 1.3125rem;
          color: #80233f;
        }
      }
    }
  }
}
</style>
