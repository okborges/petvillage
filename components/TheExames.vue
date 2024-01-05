<template>
    <div class="container" id="servicos">
        <article>
            <img src="../assets/imgs/flouffy-g2FtlFrc164-unsplash.jpg" />
            <div>
                <h2>Realizamos exames complementares</h2>
                <p>
                    Problemas alérgicos são comuns em cães. Consultar um
                    especialista para diagnóstico e exames é crucial. Isso ajuda
                    a identificar a patologia e a determinar o tratamento
                    correto, garantindo a saúde do seu animal de estimação.
                </p>
                <div class="card">
                    <h3>Cuidado Personalizado</h3>
                    <span
                        >Oferecemos um atendimento personalizado para cada
                        animal.</span
                    >
                </div>
                <div class="card">
                    <h3>Profissional especialista</h3>
                    <span
                        >Avaliação e tratamento de doenças por
                        especialistas.</span
                    >
                </div>
                <div class="card">
                    <h3>Excelente Serviço</h3>
                    <span
                        >Nosso compromisso é oferecer o melhor serviço possível
                        para nossos clientes.</span
                    >
                </div>
            </div>
        </article>
    </div>
</template>

<style scoped lang="scss">
article {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 2rem 0rem;

    img {
        max-width: 500px;
        width: 100%;
        border-radius: 40px 250px 300px 300px;
    }
    div {
        max-width: 500px;
        h2 {
            font-size: clamp(2.4rem, 8vw, 3.5rem);
            font-family: Playfair Display;
            font-weight: 600;
            color: #121212;
            padding-bottom: 2rem;
        }
        p {
            font-size: 1rem;
            padding-bottom: 1rem;
        }
        .card {
            padding: 1.5rem;
            border-radius: 30px;
            border: 2px solid #d0d7d9;
            margin-bottom: 1rem;
        }
    }
}
</style>
