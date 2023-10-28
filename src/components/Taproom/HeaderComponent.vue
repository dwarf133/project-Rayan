<template>
    <section
        :class="[{'sticky': scrolled}, 'header']" v-on:scroll="handleScroll"
    >
        <a href="#" class="logo">ТАПРУМ</a>

        <ul :class="[{'open': clickedMenu}, 'navbar']">
            <li><a href="#home">Главная</a></li>
            <li><a href="#holiday">Про ТАПРУМ</a></li>
            <li><a href="#events">События</a></li>
            <li><a href="#shop">Ассортимент</a></li>
            <li><a href="#contacts">Контакты</a></li>
        </ul>

        <div class="h-right">
            <a href="#">Последние новости тут:</a>
            <div class="h-right-socials">
                <a href="https://www.instagram.com/stepiveter/"><i class="ri-instagram-fill"></i></a>
                <a href="https://t.me/steppewindtaproom"><i class="ri-telegram-fill"></i></a>
                <a href="https://www.youtube.com/c/stepiveter"><i class="ri-youtube-fill"></i></a>
            </div>
        </div>
        <div class="bx bx-menu" id="menu-icon" v-on:click="clickedMenu = !clickedMenu"></div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            scrolled: false,
            lastPosition: 0,
            clickedMenu: false,
        }
    },
    mounted() {
        window.addEventListener("scroll", this.handleScroll);
    },
    methods: {
        handleScroll() {
            if (window.scrollY > 60) {
                this.scrolled = true;
            } else {
                this.scrolled = false;
            }

            this.lastPosition = window.scrollY;
        }
    },
}
</script>

<style scoped>
@import "../../assets/sass/style.css";
.header {
    position: fixed;
    top: 0;
    right: 0;
    z-index: 98;
    width: 100%;
    /*background: #000;*/
    background: transparent;
    padding: 27px 17%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    transition: all .50s ease;
}

.header.sticky {
    padding: 8px 17%;
    background: transparent;
    backdrop-filter: blur(20px);
}

.logo {
    font-size: 33px;
    color: #ffa343;
}

.navbar {
    display: flex;
}

.navbar a {
    margin: 15px 22px;
    font-size: 1rem;
    font-weight: 500;
    color: #fff;
    transition: all .50s ease;
    font-family: 'Nunito', sans-serif;
}

.navbar a:hover {
    color: #ffa343;
}

.h-right {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.h-right a:first-child {
    color: #fff;
    font-size: 1rem;
    margin-right: 20px;
}

.h-right a {
    vertical-align: middle;
    font-size: 20px;
    color: #fff;
    margin-right: 18px;
    margin-left: 5px;
    transition: all .50s ease;
    font-family: 'Nunito', sans-serif;
}

.h-right a:hover {
    color: #ffa343;
    transform: translateY(-3px);
}

#menu-icon {
    color: #fff;
    font-size: 30px;
    cursor: pointer;
    z-index: 10001;
    display: none;
}

@media (max-width: 1700px) {
    .header {
        padding: 18px 8%;
    }
    .header.sticky {
        padding: 7px 8%;
    }
    section {
        padding: 50px 8% 40px;
    }
}

@media (max-width: 1200px) {
    .header {
        padding: 14px 5%;
    }
    .header.sticky {
        padding: 7px 5%;
    }
    section {
        padding: 45px 5% 35px;
    }
}

@media(max-width: 1050px) {
    #menu-icon {
        display: block;
    }

    .navbar {
        position: absolute;
        width: 100%;
        height: 100vh;
        padding: 40px 60px;
        top: 0;
        bottom: 0;
        left: 100%;
        right: 0;
        display: flex;
        flex-direction: column;
        background: #000;
        transition: all .50s ease;
        justify-content: flex-start;
    }

    .navbar.open {
        left: 0;
    }

    .navbar a {
        display: block;
        color: #979797;
        padding: 0;
        margin: 0px 0px 40px 0px;
        font-size: 2.2rem;
        font-weight: 400;
    }

    .h-right {
        display: none;
    }
}

@media (max-width: 450px) {
    .header {
        padding: 12px 3%;
    }
    section {
        padding: 60px 3% 50px;
    }
}
</style>
