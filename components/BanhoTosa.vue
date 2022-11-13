<template>
  <section id="banho">
    <div class="container mx-auto px-6 grid lg:grid-cols-2">
      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">O melhor para o seu amigo você encontra aqui.</h1>
        <p class="mb-10 lg:mb-14">
          Banho e tosa realizados com muito carinho, cuidado e amor por ótimos
          profissionais, com formação, experiência e capacitados para realização
          dos serviços com segurança e excelência. <br />
          <br />
          Banhos a partir de R$50,00 <br />
          Pacotes mensais a partir de R$180,00
        </p>

        <div class="tratamentos grid grid-cols-2 gap-14">
          <div>
            <img
              class="mb-2"
              src="~/assets/icons/shampoo.svg"
              alt="shamppo"
              width="32"
              height="32"
            />
            <h2 class="mb-3">Banho</h2>
            <ul>
              <li>Banho</li>
              <li>Corte de unha</li>
              <li>Limpeza ouvido</li>
              <li>Escovação de dentes</li>
              <li>Hidratação</li>
            </ul>
          </div>

          <div>
            <img
              class="mb-2"
              src="~/assets/icons/scissors.svg"
              alt="tesoura"
              width="32"
              height="32"
            />
            <h2 class="mb-3">Tosa</h2>
            <ul>
              <li>Máquina</li>
              <li>Tesoura</li>
              <li>Higiênica</li>
              <li>Desembolo</li>
              <li>Remoção de sub-pelo</li>
            </ul>
          </div>
        </div>
      </div>

      <div class="verde pt-16 grid justify-center">
        <div class="flic">
          <Flicking
            :options="{
              circular: true,
            }"
            :plugins="plugins"
          >
            <img src="~/assets/img/banho.webp" alt="foto cachorro 1" />
            <img src="~/assets/img/banho1.webp" alt="foto cachorro 2" />
            <img src="~/assets/img/banho2.webp" alt="foto cachorro 3" />
            <img src="~/assets/img/banho3.webp" alt="foto cachorro 4" />
            <img src="~/assets/img/banho4.webp" alt="foto cachorro 5" />
          </Flicking>
        </div>
        <p class="text-center py-10 px-2">
          Utilizamos produtos de primeira linha, evitando irritação à pele,
          cuidado especial à pelagem, proporcionando um resultado de qualidade e
          durabilidade superior em serviço Pet.
        </p>
        <button class="justify-self-center mb-6">
          <a href="https://wa.me/5511981287333" target="_blank"
            >Marcar Banho | Tosa</a
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
      object-position: top;
    }
  }
  .verde {
    background-color: #ff457e;
    button {
      padding: 0.875rem 1.5rem;
      background: #40111f;
      border: 0.25rem solid #40111f;
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
      border: 0.25rem solid #7f223f;
      transform: scale(1.02);
    }
    p {
      font-family: 'Barlow';
      font-weight: 600;
      font-size: 1.25rem;
      line-height: 1.875rem;
      color: #40111f;
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
      color: #40111f;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 1.25rem;
      line-height: 1.6875rem;
      color: #80233f;
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
