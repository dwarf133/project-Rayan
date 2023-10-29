<template>
  <section class="holiday" id="holiday">
    <div class="holiday-img">
      <img src="../../taproom/assets/img/cat.jpg" alt="barrels">
    </div>

    <div class="holiday-text">
      <h2>Возможности</h2>
      <p>
        профтестиум - Lorem ipsum dolor sit amet, consectetur adipisicing elit. A, alias amet at beatae consequuntur
        culpa cupiditate deleniti deserunt dolor enim, eos et fuga fugit incidunt ipsam labore magnam maiores
        necessitatibus nesciunt possimus, quasi quidem tempora ullam vitae voluptatem? Delectus, sint.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium ad atque cum, cupiditate fuga harum iste laudantium magnam natus necessitatibus nulla numquam odit provident quidem quis reiciendis sapiente veniam. Alias aperiam aut doloremque earum enim expedita itaque iure, magni maxime molestias necessitatibus nihil numquam officia repellat reprehenderit sequi sunt totam? Dolorum illo itaque minus perspiciatis repudiandae saepe sed soluta veritatis.
      </p>
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

.holiday {
  background: #000;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  align-items: center;
  gap: 9rem;
}

.holiday-img img {
  width: 100%;
  height: auto;
  border-radius: 10px;
}

.holiday-text h5 {
  font-size: 22px;
  font-weight: 600;
  color: #ffa343;
  text-transform: uppercase;
  letter-spacing: 6px;
  margin-bottom: 20px;
}

.holiday-text h2 {
  font-size: 3rem;
  font-weight: 800;
  line-height: 1.2;
  margin-bottom: 25px;
  color: #ffa343;
}

.holiday-text p {
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

  .holiday-text p:last-child {
    margin-bottom: 0;
  }
}
</style>
