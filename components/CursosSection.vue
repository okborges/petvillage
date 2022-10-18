<template>
  <section id="cursos" class="my-16 lg:my-24">
    <div class="container mx-auto px-6">
      <h1 class="pb-8">Cursos</h1>
      <div class="grid gap-10 lg:grid-cols-4">
        <div class="cards cor-1 grid justify-center">
          <h2>Módulo 1 - Banho</h2>
          <h3>R$500,00</h3>
          <ul>
            <li>Banho ( passo a passo)</li>
            <li>Escovação de pelos e Dentes</li>
            <li>Hidratação / contenção</li>
            <li>Tosa higienica</li>
            <li>Finalização ( penteados)</li>
            <li>Gatos</li>
            <li>5 aulas</li>
          </ul>
          <a href="https://wa.me/5511984278119" target="_blank">inscreva-se</a>
        </div>

        <div class="cards cor-2 grid justify-center">
          <h2>Módulo 2 - Tosa (básico)</h2>
          <h3>R$550,00</h3>
          <ul>
            <li>Tosa higiênica</li>
            <li>Treinamento com a tesoura</li>
            <li>Tosa geral</li>
            <li>Tosa tesoura ( polimento)</li>
            <li>Tosa bebe</li>
            <li>Tosa bebe</li>
            <li>5 aulas</li>
          </ul>
          <!-- <p>
            *Necessario trazer o cão modelo para aula de tosa bebe (Curso só
            pode ser feito pra quem já é banhista)
          </p> -->
          <a href="https://wa.me/5511984278119" target="_blank">inscreva-se</a>
        </div>

        <div class="cards cor-3 grid justify-center">
          <h2>Modulo 3 - Banho e Tosa</h2>
          <h3>R$850,00</h3>
          <ul>
            <li>Banho passo a passo</li>
            <li>escovaçao de pelos e Dentes</li>
            <li>Hidratação / contenção</li>
            <li>Cuidados com os tipos de pelos</li>
            <li>Tosa higienica</li>
            <li>Treinamento com Tesoura</li>
            <li>Tosa Tesoura (polimento)</li>
            <li>Banho Terapeutico</li>
            <li>finalizaçao e penteados</li>
            <li>Gatos</li>
            <li>8 aulas</li>
          </ul>
          <a href="https://wa.me/5511984278119" target="_blank">inscreva-se</a>
        </div>

        <div class="cards cor-4 grid justify-center">
          <h2>Módulo - 4 Banho e Tosa + especializaçao em tosa bebe</h2>
          <h3>R$1.000,00</h3>
          <ul>
            <li>Banho ( passo a passo)</li>
            <li>Escovação de pelos e Dentes</li>
            <li>Hidratação / contenção</li>
            <li>Tosa higienica</li>
            <li>Treinamento com Tesoura</li>
            <li>Tosa geral</li>
            <li>Tosa Tesoura (polimento)</li>
            <li>Banho Terapeutico</li>
            <li>tosa bebe</li>
            <li>Finalização ( penteados)</li>
            <li>Gato</li>
            <li>9 aulas</li>
          </ul>
          <!-- <p>Ou 950,00 com vc trazendo o cão modelo para aula de tosa bebe</p> -->
          <a href="https://wa.me/5511984278119" target="_blank">inscreva-se</a>
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
  h1 {
    font-family: 'Fraunces';
    font-weight: 700;
    font-size: 36px;
    text-align: center;
  }

  .cards {
    border-radius: 20px;
    padding: 30px;
    grid-template-rows: 0.5fr 0.5fr 3fr 0.5fr;
    h2 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 24px;
      line-height: 30px;
      padding-bottom: 20px;
    }
    h3 {
      font-family: 'Fraunces';
      font-weight: 700;
      font-size: 28px;
      line-height: 35px;
      padding-bottom: 30px;
      text-decoration: underline;
    }
    a {
      color: #ffffff;
      box-shadow: 1px 2px 6px rgba(0, 0, 0, 0.4);
      border-radius: 22px;
      margin-bottom: 30px;
      font-family: 'Quicksand';
      font-weight: 700;
      height: fit-content;
      padding: 10px;
      text-align: center;
      transition: 0.2s;
    }

    ul {
      font-family: 'Barlow';
      font-weight: 500;
      font-size: 16px;
      line-height: 26px;
      list-style: inside;
    }
  }
  .cor-1 {
    background: #b5e4db;
    color: #0f1a16;

    a {
      background: #142721;
      border: 0.25rem solid #142721;
    }
    a:hover {
      border: 0.25rem solid #126554;
      transform: scale(1.02);
    }
  }

  .cor-2 {
    background: #f98eaf;
    color: #40111f;

    a {
      background: #40111f;
      border: 0.25rem solid #40111f;
    }
    a:hover {
      border: 0.25rem solid #7f223f;
      transform: scale(1.02);
    }
  }

  .cor-3 {
    background: #f0d95f;
    color: #2d2602;

    a {
      background: #2d2602;
      border: 0.25rem solid #2d2602;
    }
    a:hover {
      border: 0.25rem solid #655712;
      transform: scale(1.02);
    }
  }

  .cor-4 {
    background: #ffb186;
    color: #3d271b;

    a {
      background: #3d271b;
      border: 0.25rem solid #3d271b;
    }
    a:hover {
      border: 0.25rem solid #a95b2f;
      transform: scale(1.02);
    }
  }
}
</style>
