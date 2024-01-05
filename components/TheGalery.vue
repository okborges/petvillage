<template>
    <section>
        <div class="container grid">
            <div class="cards">
                <img src="../assets/imgs/Citologia.png" alt="" />
                <p>Citologia e raspado de pele</p>
            </div>
            <div class="cards">
                <img src="../assets/imgs/vet2.png" alt="" />
                <p>Cultura fúngica</p>
            </div>
            <div class="cards">
                <img src="../assets/imgs/wood.png" alt="" />
                <p>Lâmpada de Wood</p>
            </div>
            <div class="cards">
                <img src="../assets/imgs/vet3.png" alt="" />
                <p>Tricograma corado</p>
            </div>
            <div class="cards">
                <img src="../assets/imgs/Prick test.png" alt="" />
                <p>
                    Prick test para alérgenos ambientais, alimentares, Patch
                    test
                </p>
            </div>
            <div class="cards">
                <img src="../assets/imgs/Imunoterapia.png" alt="" />
                <p>Imunoterapia alérgeno especifica</p>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(340px, 1fr));
    justify-items: center;
    gap: 1rem;
    .cards {
        max-width: 377px;
        background-color: #55c8bf;
        text-align: center;
        border-radius: 50px;
        img {
            width: 100%;
        }
        p {
            padding: 1rem;
            color: #ffffff;
        }
    }
}
</style>
