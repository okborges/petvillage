<template>
  <section>
    <div class="container mx-auto px-6 grid lg:grid-cols-2">
      <div class="verde pt-16 grid justify-center">
        <img class="" src="~/assets/img/derma.png" alt="" />
        <button class="justify-self-center mb-6">
          <a href="https://wa.me/5511981287333" target="_blank"
            >Marcar consulta</a
          >
        </button>
      </div>

      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">Dermatologia e Alergologia Veterinária</h1>
        <p class="mb-14">
          A pele é o maior órgão do corpo e as patologias de pele requerem uma
          atenção especial e especializada , quadros alérgicos são problemas que
          afetam uma grande parte dos cães nos dias atuais por isso é tão
          importante procurar um especialista qualificado para ajudar a
          diagnosticar e controlar está e outras patologias da pele.
        </p>

        <div class="tratamentos grid lg:grid-cols-2 gap-14">
          <div>
            <img class="mb-2" src="~/assets/icons/cruz-medica.svg" alt="" />
            <h2 class="mb-3">Realizamos exames complementares</h2>
            <ul>
              <li>Citologia raspado de pele</li>
              <li>Cultura fúngica</li>
              <li>Lâmpada de Wood</li>
              <li>Tricograma</li>
            </ul>
          </div>

          <div>
            <img class="mb-2" src="~/assets/icons/pills.svg" alt="" />
            <h2 class="mb-3">Testes alérgicos</h2>
            <ul>
              <li>Prick test para alergenos ambientais e alimentares</li>
              <li>Imunoterapia alergeno especifica.</li>
            </ul>
          </div>
        </div>
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
    background-color: #73c1b1;
    button {
      padding: 14px 24px;
      background: #142721;
      border: 0.25rem solid #142721;
      box-shadow: 0.1875rem 0.25rem 0.6875rem rgba(0, 0, 0, 0.4);
      border-radius: 2.5rem;
      font-size: 1.25rem;
      font-weight: 700;
      color: #ffffff;
      width: max-content;
      height: fit-content;
    }
    button:hover {
      border: 0.25rem solid #126554;
      transition: 0.2s;
    }
  }

  .direita {
    max-width: 530px;
    h1 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 36px;
      line-height: 54px;
      color: #0f1a16;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 18px;
      line-height: 27px;
      color: #1f332c;
    }

    .tratamentos {
      h2 {
        font-family: 'Fraunces';
        font-weight: 700;
        font-size: 20px;
        line-height: 28px;
        color: #0f1a16;
      }
      ul {
        list-style: inside;
        li {
          font-family: 'Barlow';
          font-weight: 500;
          font-size: 14px;
          line-height: 21px;
          color: #1f332c;
        }
      }
    }
  }
}
</style>
