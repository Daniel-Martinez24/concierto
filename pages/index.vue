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
    <div id="invitados">
      <div>
        <h3 class="fecha">INVITADOS ESPECIALES</h3>
        <br>
        <div class="cards">
          <div class="hijo">
            <div>
              <Card titulo="LEVANTANDO ALTARES" lugar="Desde Monterrey"/>
            </div>
          </div>
          <div class="hijo">
            <div>
              <Card titulo="TANIA GARCíA" lugar="Desde Veracruz"/>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="descripcion">
      <div>
        <h3>UNA NOCHE DE ADORACIÓN CON</h3>
        <h2>GRUPO BARAK</h2>
        <div>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
        </div>
        <p>Nominados al Grammy Latino 2017</p>
        <p>Llegan desde República Dominicana</p>
        <p>Presentando su nuevo álbun SHEKINAH</p>
        <br>
        <br>
        <p id="hash"><strong>#ShekinahLiveTour2020</strong></p>
      </div>
    </div>
    <div class="entradas">
      <div>
        <h1>ADQUIERE TUS ENTRADAS</h1>
        <br>
        <p>¡Ahora puedes comprar tus boletos online!</p>
        <p>Aceptamos tarjetas de crédito y débito,</p>
        <p>además de pago en tiendas oxxo.</p>
      </div>
    </div>
    <p>hello</p>
  </div>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
import Card from '~/components/Card.vue'

export default {
  components: {
    Navbar,
    Card
  }
}
</script>

<style>
/*entradas*/
.entradas {
  background-color: #2D2D2D;
  color: #fff;
  min-height: 60vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.entradas h1 {
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 28px;
}

/*descripcion*/
.descripcion {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: #fff;

  background: url('https://us.123rf.com/450wm/malven/malven1611/malven161100122/66379360-fondo-de-color-gris-textura-suave-monótono-de-papel-mate.jpg?ver=6');
}
.descripcion h2{
  font-size: 36px;
}

/* invitados */
#invitados {
  background-color: #2D2D2D;
  min-height: 30vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.cards {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.cards .hijo {
  margin-left: 10vh;
  margin-right: 10vh;
  margin-top: 0vh;
}
/*main */
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
  /* invitados */
  #invitados {
    min-height: 40vh;
  }
  .cards {
    display: block;
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  .cards .hijo {
    margin: 2vh;
    margin-top: 0%;
    margin-left: 0%;
    margin-right: 0%;
  }
  /* main */
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
