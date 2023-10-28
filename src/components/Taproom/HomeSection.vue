<template>
    <section class="home" id="home">
        <div class="home-text">
            <p>Единая платформа для обучения
              <br>и тестирования сотрудников рабочих
              профессий посредством
            </p>
            <h1>ПрофТестиум</h1>
            <h5>VR-инструменты<br> симулирующих реальные ситуации в рамках конкретного предприятия.</h5>
            <a href="/catalog" class="btn">Тарифы</a>
        </div>
    </section>
</template>

<script>
    export default {
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>

<style scoped>
@import "../../taproom/assets/sass/style.css";

section {
    padding: 70px 17% 60px;
}

.home {
    position: relative;
    height: 100vh;
    width: 100%;
    background-image: linear-gradient(to left, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.3)), url('../../taproom/assets/img/mainbg.jpg');
    background-size: cover;
    /*background-attachment: fixed;*/
    background-position: bottom center;
    display: flex;
    align-items: center;
    justify-content: center;
}

.home-text {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.home-text h5 {
    font-size: 2rem;
    font-weight: 400;
    text-transform: uppercase;
    color: #ffffff;
    text-align: center;
    letter-spacing: 1px;
    margin-bottom: 130px;
}

.home-text h1 {
    font-size: 6rem;
    font-weight: 400;
    line-height: 1.2;
    margin-bottom: 20px;
    /*margin-top: 160px;*/
    color: #fff;
    text-align: center;
    letter-spacing: 15px;
}

.home-text p {
    font-size: 1.6rem;
    font-weight: 500;
    line-height: 30px;
    margin-bottom: 130px;
    color: #a2a2a2;
    text-align: center;
}

.btn {
    display: inline-block;
    padding: 5px 40px;
    background: #ffa343;
    color: #000;
    font-size: 35px;
    font-weight: 400;
    border: 2px solid transparent;
    transition: all .50s ease;
    cursor: pointer;
    border-radius: 15px;
}

.btn:hover {
    transform: translateX(10px);
    border: 2px solid #fff;
    background: transparent;
    color: #fff;
}

@media (max-width: 1700px) {
    section {
        padding: 50px 8% 40px;
    }
}

@media (max-width: 1200px) {
    section {
        padding: 45px 5% 35px;
    }
    .home {
        height: 90vh;
    }
    .home-text h5 {
        font-size: 3rem;
        margin-bottom: 100px;
    }
    .home-text h1 {
        font-size: 5rem;
    }
    .home-text p {
        margin-bottom: 100px;
    }
}

@media (max-width: 600px) {
    .home {
        height: 85vh;
    }
    .home-text h1 {
        font-size: 3rem;
    }
    .home-text h5 {
        font-size: 2.6rem;
        margin-bottom: 80px;
    }
    .home-text p {
        margin-bottom: 80px;
        font-size: 1.2rem;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
    .home-text h1 {
        font-size: 3.5rem;
    }
    .home-text h5 {
        font-size: 1.5rem;
        margin-bottom: 80px;
    }
    .home-text p {
        font-size: 1.1rem;
    }
}
</style>
