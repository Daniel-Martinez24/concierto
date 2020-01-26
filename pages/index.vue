<template>
  <div>
    <Navbar class="NavBar" />
    <div class="container">
      <div>
        <h1 class="title">
          <img src="~/static/shekinahLetters.svg" alt="">
        </h1>
        <h2 class="subtitle">
          EL ARCA EN MOVIMIENTO
        </h2>
        <h3 class="fecha">
          MARZO 26
        </h3>
        <h3 class="fecha">
          DE 18:00 A 22:00 HORAS
        </h3>
        <br>
        <h3 class="lugar">
          En el Lienzo Charro "Los Tamaulipecos"
        </h3>
        <h3 class="lugar">
          Reynosa, Tamaulipas
        </h3>
        <br>
        <br>
        <el-button type="success" round>
          <strong>
            COMPRAR ENTRADAS
          </strong>
        </el-button>
      </div>
    </div>
    <p>hello</p>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'

export default {
  components: {
    Navbar
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;

  background: url('http://www.proyectosluzcasanova.org/wp-content/uploads/2017/05/violeta-escarchado-887151.jpg');
}

.title{
  display: block;
}
.title img{
  width: 30%;
}

.subtitle {
  font-weight: 900;
  font-size: 28px;
  color: #fff;
  word-spacing: 5px;
  padding-top: 15px;
  padding-bottom: 25px;
}

.fecha {
  font-weight: 900;
  font-size: 18px;
  color: #fff;
  padding-bottom: 2px;
}
.lugar {
  font-weight: 500;
  font-size: 18px;
  color: #fff;
  padding-bottom: 2px;
}

@media (max-width: 600px){
  .title img{
    width: 50%;
    padding-bottom: 10%;
  }
  .subtitle {
    display: none;
  }
  .fecha {
    font-weight: 900;
    font-size: 16px;
    color: #fff;
    padding-bottom: 2px;
  }
  .lugar {
    font-weight: 500;
    font-size: 18px;
    color: #fff;
    padding-bottom: 2px;
  }
}

</style>
