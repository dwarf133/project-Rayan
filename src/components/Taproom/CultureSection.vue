<template>
  <section class="Culture">
    <div class="Culture-text">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facere, pariatur, quia. Amet asperiores debitis et id
        iure labore laboriosam minima molestias non odit. Animi atque consectetur consequuntur corporis cupiditate dicta
        dolorem eos ex in laborum minima mollitia necessitatibus neque numquam officiis pariatur quaerat quam rem
        repudiandae sapiente, similique sunt voluptatibus? Dolores itaque nulla quod soluta tempora? Ad amet autem
        fugiat mollitia neque praesentium reprehenderit? Dolores error harum ipsam ipsum minus molestiae nesciunt quas
        recusandae soluta voluptate. Accusantium hic natus non!
      </p>
    </div>

    <Splide class="Culture-img">
      <SplideSlide>
        <img src="../../taproom/assets/img/bar.png" alt="c1">
      </SplideSlide>
      <SplideSlide>
        <img src="../../taproom/assets/img/bar.png" alt="c1">
      </SplideSlide>
      <SplideSlide>
        <img src="../../taproom/assets/img/barrels2.png" alt="c1">
      </SplideSlide>
    </Splide>
  </section>
</template>

<script>
import {Splide, SplideSlide} from '@splidejs/vue-splide';

export default {
  components: {
    Splide,
    SplideSlide,
  }
}

</script>

<style scoped>
@import "../../taproom/assets/sass/style.css";

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
  font-size: 1.3rem;
  font-weight: 500;
  line-height: 30px;
  color: #ffffff;
  margin-bottom: 35px;
  font-family: 'Nunito', sans-serif;
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

@media (max-width: 1050px) {
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
    padding: 0 3% 50px;
  }
}
</style>
