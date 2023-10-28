<template>
    <section class="tour" id="events">
        <div class="center-text">
            <h2>События в тапруме</h2>
        </div>
        <div class="tour-text">
            <p>
                В стенах тапрума мы проводим различные мероприятия: дегустации, лекции, выставки, экскурсии,
                выступления dj, интеллектуальные вечера.
            </p>
        </div>

        <div class="tour-content">
            <div class="box">
                <img src="../../taproom/assets/img/fun1.png" alt="t1">
                <div class="content">
                    <p>Лекция про вкусы: от оренбургского бармена николая карпова <br> 19 авг 2023</p>
                </div>
            </div>

            <div class="box">
                <img src="../../taproom/assets/img/fun2.png" alt="t2">
                <div class="content">
                    <p>Пивная йога в летнике тапрума <br> 23 авг 2023</p>
                </div>
            </div>

            <div class="box">
                <img src="../../taproom/assets/img/fun3.png" alt="t3">
                <div class="content">
                    <p>Фестиваль "Степная история" <br> 26 пивоварен, сидрерий и медоварен со всей россии <br> 18 - 20 августа 2023</p>
                </div>
            </div>
            <div class="box">
                <img src="../../taproom/assets/img/fun4.png" alt="t4">
                <div class="content">
                    <p>Здесь могла быть ваша реклама!</p>
                </div>
            </div>
        </div>

        <div class="center-btn">
            <a href="mailto:taproom@тапрум.рф" class="btn">Предложить событие</a>
            <a href="https://t.me/steppewindtaproom" class="btn">Быть в курсе событий</a>
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
    grid-template-columns: repeat(auto-fit, minmax(150px, auto));
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
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    display: flex;
    text-align: center;
    margin-top: 4rem;
    gap: 30px;
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

.content {
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    position: absolute;
    background: rgba(0, 0, 0, 0.6);
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    opacity: 0;
    transition: 0.5s;
    color: #fff;
    font-size: 20px;
    padding: 10px;
    text-align: center;
    cursor: pointer;
}

.content:hover {
    opacity: 1;
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
        grid-template-columns: 2fr;
    }
    .tour-content {
        gap: 1rem;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
