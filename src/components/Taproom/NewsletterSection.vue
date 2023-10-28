<template>
    <section class="newsletter">
        <div class="newsletter-content">
            <div class="newsletter-text">
                <h2>Подпишись на нашу рассылку</h2>
                <p>Узнайте первыми о новых сортах Steppe & Wind Meadery!</p>
            </div>

            <form action="">
                <input type="email" placeholder="Введите вашу почту..." required>
                <input type="submit" value="Подписаться" class="btn">
            </form>
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

.newsletter {
    /*background: #000;*/
    background-image: linear-gradient(to left, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.3)), url('../../assets/img/newsletter.jpg');
    /*background-attachment: fixed;*/
    background-position: center;
    background-size: cover;
}

.newsletter-content {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    gap: 2rem;
}

.newsletter-text h2 {
    font-size: 2.7rem;
    font-weight: 800;
    margin-bottom: 15px;
    color: #ffa343;
}

.newsletter-text p {
    font-size: 1.7rem;
    font-weight: 500;
    color: #ffffffab;
}

.newsletter-content form {
    display: grid;
    grid-template-columns: 1fr 0.4fr;
    gap: 1rem;
}

.newsletter-content form input:first-child {
    padding: 0 15px;
    background: #202020;
    font-size: 1.7rem;
    color: #fff;
    border-radius: 5px;
    font-family: 'Nunito', sans-serif;
    border: 1px solid #ffffff;
}

.btn {
    display: inline-block;
    padding: 2px 40px;
    background: #ffa343;
    color: #000;
    font-size: 30px;
    font-weight: 400;
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

@media (max-width: 800px) {
    .newsletter-content {
        grid-template-columns: 1fr;
    }

    .newsletter-content form {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 450px) {
    section {
        padding: 60px 3% 50px;
    }
}
</style>
