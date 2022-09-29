<template>
  <section id="creche">
    <div class="container mx-auto px-6 grid lg:grid-cols-2 items-center">
      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">Creche</h1>
        <p class="mb-0 lg:mb-14">
          As atividades são dirigidas para a socialização com outros Pets,
          liberdade para brincar e correr, saúde mental, alimentação e cuidados,
          conforme estão acostumados em casa, sempre respeitando a
          individualidade e natureza de cada um. Visite-nos !
        </p>
      </div>

      <div class="verde pt-16 grid justify-center">
        <img class="" src="~/assets/img/creche.png" alt="" />
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
export default {};
</script>

<style lang="scss" scoped>
section {
  .verde {
    background-color: #ffa370;
    button {
      padding: 14px 24px;
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
      font-size: 20px;
      line-height: 30px;
      color: #452310;
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
      color: #3d271b;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 20px;
      line-height: 27px;
      color: #814321;
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
