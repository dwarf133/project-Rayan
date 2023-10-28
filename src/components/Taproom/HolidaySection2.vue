<template>
    <section class="new-holiday" id="contacts">
        <div class="center-text">
            <h2>Контакты</h2>
        </div>
        <div class="new-holiday-text">
            <p>Оренбург, ул. Березка 22. Режим работы: пт - сб, 20:00 - 02:00</p>
        </div>
        <div class="holiday">
            <div class="holiday-img">
                <img src="../../assets/img/toilets.png" alt="toilets">
            </div>

            <div class="holiday-text">
                <div class="step-and-wind">
                    <h5><a href="https://vk.com/stepiveter">Медоварня "Степь и Ветер" вконтакте</a></h5>
                    <h5><a href="https://www.youtube.com/c/stepiveter">Медоварня "Степь и Ветер" на ютуб</a></h5>
                    <h5><a href="https://t.me/stepiveter1">Медоварня "Степь и Ветер" в телеграм</a></h5>
                    <h5><a href="https://www.instagram.com/stepiveter/">Медоварня "Степь и Ветер" в инсте</a></h5>
                    <h5><a href="https://stepiveter.ru/">Медоварня "Степь и Ветер" на сайте</a></h5>
                </div>
                <div class="taproom">
                    <h5><a href="#">Тапрум вконтакте</a></h5>
                    <h5><a href="#">Тапрум в телеграм</a></h5>
                    <h5><a href="#">Тапрум в инсте</a></h5>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

</script>

<style scoped>
@import "../../assets/sass/style.css";

a  {
    color: #fff;
}

h5 {
    text-decoration: none;
    color: #fff;
    transition: all .50s ease;
}

.holiday-text h5:hover {
    color: #ffa343;
    transform: translateY(-3px);
}

.holiday-text a:hover {
    color: #ffa343;
    transform: translateY(-3px);
}

section {
    padding: 70px 17% 60px;
}

.new-holiday {
    background: #000;
}

.center-text h2 {
    /*text-align: center;*/
    font-size: 3rem;
    color: #ffa343;
    margin-bottom: 25px;
}

.new-holiday-text p {
    font-size: 1.3rem;
    font-weight: 500;
    line-height: 30px;
    color: #ffffff;
    margin-bottom: 35px;
    font-family: 'Nunito', sans-serif;
}

.holiday {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 9rem;
}

.holiday-img img {
    width: 100%;
    height: auto;
    border-radius: 10px;
    border: 2px solid #ffa343;
}

.holiday-text h5 {
    font-size: 26px;
    font-weight: 400;
    color: #ffa343;
    text-transform: uppercase;
    margin-bottom: 10px;
}

.holiday-text h2 {
    font-size: 3rem;
    font-weight: 800;
    line-height: 1.2;
    margin-bottom: 25px;
    color: #fff;
}

.holiday-text p {
    font-size: 1rem;
    font-weight: 500;
    line-height: 30px;
    color: #ffffffab;
    margin-bottom: 35px;
}

.holiday-text .step-and-wind {
    margin-bottom: 60px;
}

.btn {
    display: inline-block;
    padding: 13px 40px;
    background: #ffa343;
    color: #000;
    font-size: 15px;
    font-weight: 600;
    border: 2px solid transparent;
    border-radius: 5px;
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
    .holiday {
        gap: 3rem;
    }
}

@media (max-width: 800px) {
    .holiday {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
