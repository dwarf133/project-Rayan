<template>
    <section class="Culture">
        <div class="Culture-text">
            <h5>Четвертый блок</h5>
            <h2>Четвертый блок</h2>
            <p>how to make complete responsive tours and travel website designs using HTML CSS from scratch.
                Responsive travel website design using HTML CSS. Responsive website HTML CSS.</p>
            <a href="#" class="btn">Читать далее</a>
        </div>

        <div class="Culture-img">
            <img src="../../assets/img/barrels2.png" alt="c1">
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

.Culture {
    background: #000;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 9rem;
}

.Culture-img img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

.Culture-text h5 {
    font-size: 22px;
    font-weight: 600;
    color: #ffa343;
    text-transform: uppercase;
    letter-spacing: 6px;
    margin-bottom: 20px;
}

.Culture-text h2 {
    font-size: 3rem;
    font-weight: 800;
    line-height: 1.2;
    margin-bottom: 25px;
    color: #fff;
}

.Culture-text p {
    font-size: 1rem;
    font-weight: 500;
    line-height: 30px;
    color: #ffffffab;
    margin-bottom: 35px;
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
    .Culture {
        gap: 3rem;
    }
}

@media (max-width: 800px) {
    .Culture {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
