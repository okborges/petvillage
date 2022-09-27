<template>
  <section id="banho">
    <div class="container mx-auto px-6 grid lg:grid-cols-2">
      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">O melhor para o seu amigo você encontra aqui.</h1>
        <p class="mb-14">
          Banho e tosa realizados com muito carinho, cuidado e amor por ótimos
          profissionais, com formação, experiência e capacitados para realização
          dos serviços com segurança e excelência.
        </p>

        <div class="tratamentos grid grid-cols-2 gap-14">
          <div>
            <img class="mb-2" src="~/assets/icons/shampoo.svg" alt="" />
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
            <img class="mb-2" src="~/assets/icons/scissors.svg" alt="" />
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
        <img class="" src="~/assets/img/banho.png" alt="" />
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
export default {};
</script>

<style lang="scss" scoped>
section {
  .verde {
    background-color: #ff457e;
    button {
      padding: 14px 24px;
      background: #40111f;
      border: 0.25rem solid #40111f;
      box-shadow: 0.1875rem 0.25rem 0.6875rem rgba(0, 0, 0, 0.4);
      border-radius: 2.5rem;
      font-size: 1.25rem;
      font-weight: 700;
      color: #ffffff;
      width: max-content;
      height: fit-content;
    }
    button:hover {
      border: 0.25rem solid #7f223f;
      transition: 0.2s;
    }
    p {
      font-family: 'Barlow';
      font-weight: 600;
      font-size: 20px;
      line-height: 30px;
      color: #ffffff;
      max-width: 430px;
      justify-self: center;
    }
  }

  .direita {
    max-width: 530px;
    h1 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 36px;
      line-height: 54px;
      color: #40111f;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 20px;
      line-height: 27px;
      color: #80233f;
      max-width: 410px;
    }

    .tratamentos {
      h2 {
        font-family: 'Fraunces';
        font-weight: 700;
        font-size: 20px;
        line-height: 28px;
        color: #40111f;
      }
      ul {
        list-style: inside;
        li {
          font-family: 'Barlow';
          font-weight: 500;
          font-size: 14px;
          line-height: 21px;
          color: #80233f;
        }
      }
    }
  }
}
</style>
