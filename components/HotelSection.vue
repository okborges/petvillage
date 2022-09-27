<template>
  <section id="hotel">
    <div class="container mx-auto px-6 grid lg:grid-cols-2 items-center">
      <div class="verde pt-16 grid justify-center">
        <img class="" src="~/assets/img/hotel.png" alt="" />
        <p class="text-center py-10">
          Nossa experiência de mais de 12 anos, com monitores orientados a
          tratar nossos clientes como parte da família, garantem tratamento
          individualizado e focado em suas necessidades específicas.
        </p>
        <button class="justify-self-center mb-6">
          <a href="https://wa.me/5511981287333" target="_blank">Marcar Hotel</a>
        </button>
      </div>

      <div class="direita mb-12 mt-8 lg:mt-16 lg:ml-20">
        <h1 class="mb-5">Hotel e Bem estar do seu melhor amigo.</h1>
        <p class="mb-14">
          O Seu Pet é o nosso Pet - esse é um princípio de conduta que orienta
          nosso trabalho e nos dá satisfação ao garantir que os Pets a nós
          confiados são tratados com carinho, atenção, respeito, segurança e
          conforto.
        </p>
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
    background-color: #fed501;
    button {
      padding: 14px 24px;
      background: #2e2704;
      border: 0.25rem solid #2e2704;
      box-shadow: 0.1875rem 0.25rem 0.6875rem rgba(0, 0, 0, 0.4);
      border-radius: 2.5rem;
      font-size: 1.25rem;
      font-weight: 700;
      color: #ffffff;
      width: max-content;
      height: fit-content;
    }
    button:hover {
      border: 0.25rem solid #655712;
      transition: 0.2s;
    }
    img {
      justify-self: center;
    }
    p {
      max-width: 430px;
      font-family: 'Barlow';

      font-weight: 600;
      font-size: 20px;
      line-height: 30px;
      text-align: center;
      color: #2d2602;
    }
  }

  .direita {
    max-width: 530px;
    h1 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 36px;
      line-height: 54px;
      color: #2d2602;
    }
    p {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 18px;
      line-height: 27px;
      color: #2e2704;
    }
  }
}
</style>
