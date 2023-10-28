<template>
    <section class="feature">
        <div class="center-text">
            <h2>Линейка сортов</h2>
        </div>

        <div class="feature-content">
            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/first.png" alt="nap1">
                </div>
                <h4>Моносорта</h4>
            </div>

            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/second.png" alt="nap2">
                </div>
                <h4>Традиционные</h4>
            </div>

            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/third.png" alt="nap3">
                </div>
                <h4>Составные</h4>
            </div>

            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/fouth.png" alt="nap4">
                </div>
                <h4>Боше</h4>
            </div>

            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/fifth.png" alt="nap5">
                </div>
                <h4>Смузи</h4>
            </div>

            <div class="row">
                <div class="row-img">
                    <img src="../../assets/img/sixth.png" alt="nap6">
                </div>
                <h4>Безалкогольные</h4>
            </div>
        </div>
    </section>
</template>

<script>

</script>

<style scoped>
@import "../../assets/sass/style.css";

section {
    padding: 70px 17% 60px;
}

.center-text {
    text-align: center;
    font-size: 2rem;
    color: #fff;
}

.center-text h2 {
    font-size: 3rem;
    font-weight: 800;
}

.feature {
    background: #000;
}

.feature-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(150px, auto));
    text-align: center;
    gap: 3rem;
    margin-top: 5rem;
}

.row-img {
    overflow: hidden;
    width: 100px;
    height: 100px;
    margin: 0 auto 20px;
    border-radius: 50%;
    cursor: pointer;
}

.row-img img {
    width: 100%;
    display: block;
    transition: transform 0.7s;
}
.row-img img:hover {
    transform: scale(1.2);
}

.feature-content h4 {
    font-size: 17px;
    font-weight: 500;
    cursor: pointer;
    transition: all .50s ease;
    color: #fff;
}

.feature-content h4:hover {
    color: #ffa343;
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
    .feature-content {
        gap: 1.5rem;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
