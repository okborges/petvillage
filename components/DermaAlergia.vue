<template>
  <section id="derma">
    <div class="container mx-auto px-6 grid lg:grid-cols-2">
      <div class="verde pt-16 grid justify-center">
        <div class="flic">
          <Flicking
            :options="{
              circular: true,
            }"
            :plugins="plugins"
          >
            <img src="~/assets/img/derma.webp" alt="foto dermatologista 1" />
            <img src="~/assets/img/vet2.webp" alt="foto dermatologista 2" />
            <img src="~/assets/img/vet3.webp" alt="foto dermatologista 3" />
            <img src="~/assets/img/vet4.webp" alt="foto dermatologista 4" />
            <img src="~/assets/img/vet5.webp" alt="foto dermatologista 5" />
          </Flicking>
        </div>
        <button class="justify-self-center mb-6">
          <a href="https://wa.me/5511981287333" target="_blank"
            >Marcar consulta</a
          >
        </button>
      </div>

      <div
        class="direita mb-12 mt-8 order-first lg:order-none lg:mt-16 lg:ml-20"
      >
        <h1 class="mb-5">Dermatologia e Alergologia Veterinária</h1>
        <p class="mb-10 lg:mb-14">
          A pele é o maior órgão do corpo e as patologias de pele requerem uma
          atenção especial e especializada, quadros alérgicos são problemas que
          afetam uma grande parte dos cães nos dias atuais por isso é tão
          importante procurar um especialista qualificado para ajudar a
          diagnosticar e controlar está e outras patologias da pele.
        </p>

        <div class="tratamentos grid lg:grid-cols-2 gap-8 lg:gap-14">
          <div>
            <img
              class="mb-2"
              src="~/assets/icons/cruz-medica.svg"
              alt="cruz medica"
              width="29"
              height="29"
            />
            <h2 class="mb-3">Realizamos exames complementares</h2>
            <ul>
              <li>Citologia e raspado de pele</li>
              <li>Cultura fúngica</li>
              <li>Lâmpada de Wood</li>
              <li>Tricograma</li>
            </ul>
          </div>

          <div>
            <img
              class="mb-2"
              src="~/assets/icons/pills.svg"
              alt="pilulas"
              width="30"
              height="30"
            />
            <h2 class="mb-3">Testes alérgicos</h2>
            <ul>
              <li>Prick test para alérgenos ambientais e alimentares</li>
              <li>Imunoterapia alérgeno especifica.</li>
            </ul>
          </div>
        </div>
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
      object-position: top;
    }
  }
  .verde {
    background-color: #73c1b1;
    button {
      padding: 0.875rem 1.5rem;
      background: #142721;
      border: 0.25rem solid #142721;
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
      border: 0.25rem solid #126554;
      transform: scale(1.02);
    }
  }

  .direita {
    max-width: 33.125rem;
    h1 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 2.25rem;
      line-height: 3.375rem;
      color: #0f1a16;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 1.125rem;
      line-height: 1.6875rem;
      color: #1f332c;
    }

    .tratamentos {
      h2 {
        font-family: 'Fraunces';
        font-weight: 700;
        font-size: 1.25rem;
        line-height: 1.75rem;
        color: #0f1a16;
      }
      ul {
        list-style: inside;
        li {
          font-family: 'Barlow';
          font-weight: 500;
          font-size: 0.875rem;
          line-height: 1.3125rem;
          color: #1f332c;
        }
      }
    }
  }
}
</style>
