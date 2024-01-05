<script setup>
import { ref } from 'vue';

const duvidas = ref([
    {
        pergunta: 'Como posso agendar uma consulta?',
        resposta: 'Entre em contato conosco pelo whatsApp (11) 9 8128-7333',
        showResposta: false,
    },
    {
        pergunta: 'Meu animal de estimação está com coceira. O que pode ser?',
        resposta:
            'Pode ser alergia a pulgas, carrapatos entre outros tipos de alergia entre em contato para agendar uma consulta.',
        showResposta: false,
    },
    {
        pergunta: 'Quais são os exames que vocês realizam?',
        resposta: 'Citologia raspado de pele, Lâmpada de Wood, entre outros.',
        showResposta: false,
    },
]);
</script>

<template>
    <div class="container" id="duvidas">
        <section>
            <article>
                <h1>Tire suas dúvidas. <br />Confie em nosso trabalho.</h1>
                <h2>Compromisso com o bem-estar do seu animal de estimação</h2>
                <ul>
                    <li
                        v-for="(duvida, index) in duvidas"
                        :key="index"
                        @click="duvida.showResposta = !duvida.showResposta"
                    >
                        <div class="duvida_title">
                            <h3>{{ duvida.pergunta }}</h3>
                            <img src="../assets/icons/arrow-down.svg" alt="" />
                        </div>
                        <p v-if="duvida.showResposta">{{ duvida.resposta }}</p>
                    </li>
                </ul>
            </article>

            <img class="duvidas_photo" src="../assets/imgs/foto_renata.png" />
        </section>
    </div>
</template>

<style lang="scss" scoped>
section {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 2rem;
    padding: 3rem 0rem;
    article {
        h1 {
            font-family: Playfair Display;
            font-size: clamp(2.4rem, 8vw, 3.5rem);
            padding-bottom: 2.5rem;
        }
        h2 {
            color: #657172;
            font-size: 1.3rem;
            font-weight: 400;
        }
        ul {
            li {
                border-bottom: 2px solid #e5e5e5;
                padding: 1.5rem 0;
                .duvida_title {
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    gap: 1rem;
                }
                p {
                    padding-top: 1rem;
                    max-width: 500px;
                }
            }
        }
    }
    .duvidas_photo {
        width: 100%;
        max-width: 500px;
        max-height: 635px;
    }
}
</style>
