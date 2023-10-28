<template>
    <div class="popup" v-if="show">
        <div class="popup-inner">
            <h2>18 +</h2>
            <p>Уверен, что ты достаточно взрослый, чтобы быть здесь?</p>
            <div class="buttons">
                <button class="btn" @click="show = false">Мне есть 18</button>
                <button class="btn" @click="underEighteen">Мне нет 18</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: [],
    data() {
        return {
            show: true,
        }
    },
    methods: {
        underEighteen() {
            window.location.href = 'https://www.detmir.ru/';
        }
    }
}
</script>

<style scoped>
.popup {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: 99;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0.2);
    backdrop-filter: blur(10px);
}

.popup-inner {
    background-color: #ffffff;
    padding: 20px 40px;
    border-radius: 20px;
}

.popup-inner h2 {
    text-align: center;
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    color: #ff4343;
    font-size: 38px;
}

.popup-inner p {
    font-family: 'Nunito', sans-serif;
    font-weight: 700;
    text-align: center;
    font-size: 24px;
}

.popup-inner .buttons {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 20px;
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
    border: 2px solid #000000;
    background: #000000;
    color: #ffffff;
}

@media (max-width: 767px) {
    .popup-inner {
        width: 90%;
    }
    .btn {
        font-size: 26px;
    }
}
</style>
