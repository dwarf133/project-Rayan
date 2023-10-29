<template>
    <section class="footer" style="color: #ffa343;">
        <div class="footer-box">
            <h3>Контакты</h3>
            <a href="tel:+79058481865">8 (111) 111-11-11</a>
            <a>ПРОФТЕСТИУМ</a>
            <a href="../../docs/oferta.pdf" style="color: #ffa343">Оферта</a>
        </div>

        <div class="footer-box">
            <h3>Lorem ipsum dolor sit.</h3>
            <a>ИНН: 11111111111</a>
            <a>ОГРНИП: 11111 11111 11111</a>
        </div>

        <div class="footer-box">
            <h3>Lorem ipsum dolor sit amet.</h3>
            <a>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae, sed!</a>
        </div>

        <div class="footer-box">
            <h3>Social</h3>
            <div class="social">
                <a href=""><i class="ri-instagram-fill"></i></a>
                <a href=""><i class="ri-telegram-fill"></i></a>
                <a href=""><i class="ri-youtube-fill"></i></a>
            </div>
        </div>
    </section>
</template>

<script>

</script>

<style scoped>
@import "../../taproom/assets/sass/style.css";

section {
    padding: 70px 17% 60px;
}

.footer {
    background: #000;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, auto));
    gap: 2rem;
}

.footer-box {
    display: flex;
    flex-direction: column;
}

.footer-box h3 {
    font-size: 28px;
    font-weight: 600;
    margin-bottom: 15px;
}

.footer-box a {
    color: #979797;
    margin-bottom: 0.8rem;
    transition: all .50s ease;
    font-size: 22px;
    cursor: pointer;
}

.footer-box a:hover {
    transform: translateX(-5px);
    color: #fff;
}

.social a {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    height: 45px;
    width: 45px;
    background: #202020;
    color: #fff;
    font-size: 20px;
    border-radius: 50%;
    margin-right: 8px;
    transition: transform 0.6s;
}

.social a:hover {
    background: #ffa343;
    color: #000;
    transform: translateX(-4px);
}

@media (max-width: 1700px) {
    header {
        padding: 18px 8%;
    }
    section {
        padding: 50px 8% 40px;
    }
}

@media (max-width: 1200px) {
    header {
        padding: 14px 5%;
    }
    section {
        padding: 45px 5% 35px;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
