<template>
    <header class="container">
        <div class="header_items_container">
            <div class="header_item">
                <img src="../assets/icons/phone.svg" />
                <div>
                    <p>Telefone</p>
                    <span>whatsapp (11) 9 8128-7333</span>
                </div>
            </div>

            <div class="header_item">
                <img src="../assets/icons/maps.svg" />
                <div>
                    <p>R. Cel. Agenor de Camargo, 57</p>
                    <span>Centro, Santo André</span>
                </div>
            </div>

            <div class="header_item">
                <img src="../assets/icons/calendar.svg" />
                <div>
                    <p>Segunda - Sábado</p>
                    <span
                        >09:00 - 17:30 com agendamento prévio pelo
                        WhatsApp</span
                    >
                </div>
            </div>
        </div>

        <div class="social">
            <a
                href="https://api.whatsapp.com/send/?phone=%2B5511981287333&text&type=phone_number&app_absent=0"
                target="_blank"
                rel="noopener noreferrer"
            >
                <img src="../assets/icons/whatsapp.svg" width="30" />
            </a>
            <a
                href="https://www.instagram.com/petvillagedermato/"
                target="_blank"
                rel="noopener noreferrer"
            >
                <img src="../assets/icons/instagram.svg" width="30" />
            </a>
            <a
                href="https://www.facebook.com/profile.php?id=100063582402934"
                target="_blank"
                rel="noopener noreferrer"
            >
                <img src="../assets/icons/facebook.svg" width="30" />
            </a>
        </div>
    </header>
</template>

<style scoped lang="scss">
header {
    display: flex;
    padding: 32px;
    justify-content: space-between;
    .header_items_container {
        display: flex;
        flex-wrap: wrap;
        gap: 32px;
        .header_item {
            display: grid;
            grid-template-columns: max-content 1fr;
            gap: 10px;

            p {
                font-size: 16px;
                font-weight: 700;
            }
            span {
                font-size: 12px;
            }
        }
    }
    .social {
        display: flex;
        gap: 20px;
    }
}

@media (max-width: 1150px) {
    header {
        padding: 16px;
        .header_items_container {
            gap: 16px;
        }

        .social {
            display: none;
        }
    }
}
</style>
