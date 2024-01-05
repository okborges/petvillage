<template>
    <nav>
        <img src="../assets/imgs/pet_logo_branco.png" alt="" />
        <ul>
            <li>
                <a href="#servicos">Nossos serviços</a>
            </li>
            <li>
                <a href="#duvidas">Tire suas duvidas</a>
            </li>
            <li>
                <a href="#sobre">Sobre nós</a>
            </li>
            <li>
                <a
                    href="https://api.whatsapp.com/send/?phone=%2B5511981287333&text&type=phone_number&app_absent=0"
                    target="_blank"
                    >FAÇA UM AGENDAMENTO</a
                >
            </li>
        </ul>
    </nav>
</template>

<style scoped lang="scss">
nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    gap: 1rem;
    padding: 2rem 0rem;

    img {
        width: 250px;
    }

    ul {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        justify-content: center;
        gap: 2rem;
        li:last-child {
            background-color: #55c8bf;
            border-radius: 10px;
            padding: 8px 16px;
            a {
                color: #fff;
            }
        }
    }
}
</style>
