<script setup>
const datas = [
    {
        semana: 'Segunda',
        horario: '09:00 - 17:30',
    },
    {
        semana: 'Terça',
        horario: '09:00 - 17:30',
    },
    {
        semana: 'Quarta',
        horario: '09:00 - 17:30',
    },
    {
        semana: 'Quinta',
        horario: '09:00 - 17:30',
    },
    {
        semana: 'Sexta',
        horario: '09:00 - 17:30',
    },
    {
        semana: 'Sábado',
        horario: '09:00 - 12:00',
    },
    {
        semana: 'Domingo',
        horario: 'FECHADO',
    },
];
</script>

<template>
    <div class="container">
        <section>
            <div class="maps">
                <h1>RENATA JALORETTO</h1>
                <p class="sub">
                    O tratamento familiar onde o seu Pet é o nosso Pet é a base
                    do nosso trabalho.
                </p>
                <div class="icons">
                    <img src="../assets/icons/maps.svg" alt="" />
                    <p>R. Cel. Agenor de Camargo, 57 - Centro, Santo André</p>
                </div>
                <div class="icons">
                    <img src="../assets/icons/phone.svg" alt="" />
                    <p>Whatsapp: (11) 9 8128-7333</p>
                </div>
            </div>
            <div class="agenda">
                <h2>agenda</h2>
                <ul>
                    <li v-for="data in datas" :key="data.semana">
                        <p>{{ data.semana }}</p>
                        <span>{{ data.horario }}</span>
                    </li>
                </ul>
                <a
                    href="https://api.whatsapp.com/send/?phone=%2B5511981287333&text&type=phone_number&app_absent=0"
                    target="_blank"
                    >FAÇA UM AGENDAMENTO</a
                >
            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
section {
    justify-content: space-around;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    .maps {
        h1 {
            font-size: 2rem;
        }
        .sub {
            max-width: 310px;
            color: #657172;
        }
        .icons {
            display: flex;
            gap: 10px;
            align-items: flex-start;
            padding: 10px 0;
        }
    }

    .agenda {
        display: flex;
        flex-direction: column;
        width: 100%;
        max-width: 500px;
        background-color: #d0d7d9;
        padding: 5rem 5%;
        border-radius: 120px 30px 120px 120px;
        h2 {
            text-align: center;
            margin: auto;
            padding-bottom: 1rem;
        }
        ul {
            display: flex;
            flex-direction: column;
            gap: 10px;
            li {
                display: flex;
                border-radius: 10px;
                justify-content: space-between;
                padding: 0.875rem 1.75rem;
                background-color: #ffffff;
                p,
                span {
                    color: #657172;
                }
            }
        }
        a {
            background-color: #ffa1bf;
            color: #ffffff;
            padding: 1rem 1.5rem;
            margin: auto;
            font-size: 1.5rem;
            margin-top: 1rem;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
            text-align: center;
        }
        a:hover {
            background-color: #ff5d91;
        }
    }
}
</style>
