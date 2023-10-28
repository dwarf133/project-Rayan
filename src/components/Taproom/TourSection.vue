<template>
    <section class="tour" id="shop">
        <div class="center-text">
            <h2>Магазин мерча</h2>
        </div>
        <div class="tour-text">
            <p>Закажи мерч медоварни "Степь и Ветер" и ТАПРУМА в любую точку мира.</p>
        </div>

        <div class="tour-content">
            <div class="box" @click="toCatalog">
                <img src="../../assets/img/tshirt1.png" alt="t1">
                <h6>Крутейшая футболка с единорогом</h6>
                <h4>Футболки</h4>
            </div>

            <div class="box" @click="toCatalog">
                <img src="../../assets/img/tshirt2.png" alt="t2">
                <h6>АйПиОу браслет</h6>
                <h4>Браслет</h4>
            </div>

            <div class="box" @click="toCatalog">
                <img src="../../assets/img/tshirt3.png" alt="t3">
                <h6>Изогнутый стакан с единорожкой</h6>
                <h4>Бокалы</h4>
            </div>
        </div>

        <div class="center-btn">
            <a href="/catalog" class="btn">В магазин</a>
        </div>
    </section>
</template>

<script>
export default {
    methods: {
        toCatalog() {
            window.location.href = '/catalog';
        },
    }
}
</script>

<style scoped>
@import "../../assets/sass/style.css";

section {
    padding: 70px 17% 60px;
}

.tour {
    background: #000;
}

.center-text {
    /*text-align: center;*/
    font-size: 2rem;
    color: #ffa343;
    margin-bottom: 25px;
}

.center-text h2 {
    font-size: 3rem;
    font-weight: 800;
}

.tour-text p {
    font-size: 1.3rem;
    font-weight: 500;
    line-height: 30px;
    color: #ffffff;
    margin-bottom: 35px;
    font-family: 'Nunito', sans-serif;
}

.tour-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, auto));
    align-items: center;
    gap: 3rem;
    margin-top: 5rem;
}

.box {
    position: relative;
}

.box img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 10px;
    filter: brightness(70%);
    transition: all .3s cubic-bezier(.499,.05,.55,.95);
    will-change: filter;
    display: block;
}

.box h6 {
    position: absolute;
    left: 25px;
    bottom: 65px;
    font-size: 18px;
    font-weight: 500;
    color: #fff;
    font-family: 'Nunito', sans-serif;
}

.box h4 {
    position: absolute;
    left: 25px;
    bottom: 95px;
    font-size: 30px;
    font-weight: 400;
    color: #fff;
}

.box img:hover {
    filter: brightness(90%) hue-rotate(50deg);
    transform: scale(1.04);
    cursor: pointer;
}

.center-btn {
    text-align: center;
    margin-top: 4rem;
}

.btn {
    display: inline-block;
    padding: 2px 40px;
    background: #ffa343;
    color: #000;
    font-size: 35px;
    font-weight: 400;
    border: 2px solid transparent;
    border-radius: 15px;
    transition: all .50s ease;
    cursor: pointer;
}

.btn:hover {
    transform: translateX(10px);
    border: 2px solid #fff;
    background: transparent;
    color: #fff;
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

@media(max-width: 1050px) {
    .tour {
        gap: 3rem;
    }
}

@media (max-width: 800px) {
    .tour {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
