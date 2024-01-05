<template>
    <div class="container">
        <section>
            <img src="../assets/imgs/fall_foto.png" />
            <div>
                <h1>
                    Yorkshire coçava olhos e ouvidos, tratamentos caros
                    falharam. Dra. Renata resolveu tudo com exelência.
                </h1>
                <p>Alda Rita</p>
                <span>Cliente de Longa data</span>
            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
section {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    align-items: center;
    background-color: #a3b2bf;
    border-radius: 30px 120px 120px 30px;
    padding: 5% 8%;

    img {
        width: 100%;
        max-width: 300px;
    }
    div {
        max-width: 575px;
        h1 {
            font-size: clamp(1.4rem, 8vw, 2.5rem);
            padding-bottom: 2rem;
            position: relative;
            z-index: 2;
        }
        h1::before {
            content: '';
            display: inline-block;
            width: 160px;
            height: 160px;
            background: url('../assets/icons/aspas.svg') center/contain
                no-repeat;
            margin-right: 8px;
            position: absolute;
            z-index: -1;
            top: -80px;
            left: -50px;
        }
        p {
            font-size: 2rem;
            font-weight: 400;
            padding-bottom: 0.5rem;
        }
        span {
            font-size: 1.5rem;
            color: #657172;
            font-weight: 400;
        }
    }
}
</style>
