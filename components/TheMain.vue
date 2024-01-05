<template>
    <section>
        <div class="container">
            <TheNav />

            <article>
                <div>
                    <h1>Dermatologia e Alergologia Veterinária</h1>
                    <h2>
                        A pele, maior órgão do corpo, merece atenção especial.
                    </h2>
                    <p>
                        Seu amigo tem problemas de pele?
                        <a
                            href="https://api.whatsapp.com/send/?phone=%2B5511981287333&text&type=phone_number&app_absent=0"
                            target="_blank"
                        >
                            Agende uma consulta!
                        </a>
                    </p>
                </div>
                <img class="dog" src="../assets/imgs/dogHome.png" />
            </article>
        </div>
    </section>
</template>

<style scoped lang="scss">
section {
    background-image: url('../assets/icons/bg-rosa.svg');
    width: 100%;
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 0px 0px 80px 80px;

    article {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        justify-content: space-around;

        div {
            max-width: 426px;

            h1 {
                font-size: clamp(3rem, 8vw, 4rem);
                font-weight: 700;
                color: #24284c;
                font-family: 'Playfair Display', serif;
            }
            h2,
            p {
                font-size: 22px;
                color: #333333;
                padding-top: 1rem;
                a {
                    text-decoration: underline;
                }
            }
        }
        img {
            width: 100%;
            max-width: 417px;
        }
    }
}
</style>
