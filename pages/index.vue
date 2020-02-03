<template>
  <div>
    <Navbar class="NavBar" />
    <video id = "video" loop=»loop» autoplay=»autoplay» src="~/static/video.webm"></video>
    <div class="container">
      <div>
        <br>
        <br>
        <br>
        <h1 class="title">
          <img style="z-index:100;" src="~/static/shekinahLetters.svg" alt="">
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
        <el-button type="success" round>
          <strong>
            COMPRAR ENTRADAS
          </strong>
        </el-button>
      </div>
    </div>
    <div id="invitados">
      <div>
        <h3>INVITADOS ESPECIALES</h3>
        <br>
        <div class="cards">
          <div class="hijo">
            <div>
              <Card imagen='primera' titulo="LEVANTANDO ALTARES" lugar="Desde Monterrey"/>
            </div>
          </div>
          <div class="hijo">
            <div>
              <Card imagen='que' titulo="TANIA GARCíA" lugar="Desde Veracruz"/>
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
          <div class="espacios">
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
          <br>
          <br>
          <br>
          <br>
          <br>
        </div>
        <p>Nominados al Grammy Latino 2017</p>
        <p>Llegan desde República Dominicana</p>
        <p>Presentando su nuevo álbun SHEKINAH</p>
        <div class="espacios">
          <br>
        </div>
        <br>
        <p><strong>#ShekinahLiveTour2020</strong></p>
      </div>
    </div>
    <div class="entradas">
      <div>
        <h1>ADQUIERE TUS ENTRADAS</h1>
        <br>
        <p>¡Ahora puedes comprar tus boletos online!</p>
        <p>Aceptamos tarjetas de crédito y débito,</p>
        <p>además de pago en tiendas oxxo.</p>
        <br>
        <div class="reja">
          <Boletos
            v-if="pantalla > 600"
            typeBoton="success"
            nombreZona="RUEDO"
            numeroZona="ZONA 1"
            :textBoton="comprar[0]"
            id="zona1"
          />
          <Boletos
            v-else
            typeBoton="success"
            nombreZona="RUEDO"
            numeroZona="ZONA 1"
            :textBoton="comprar[1]"
            id="zona1"
          />
          <Boletos
            typeBoton="info"
            nombreZona="BUTACAS"
            numeroZona="ZONA 2"
            textBoton="AGOTADO"
            id="zona2"
          />
        </div>
      </div>
    </div>
    <div class="ubicacion">
      <Mapa class="mapa" />
    </div>
    <div class="footer">
      <div class="sigueMt5">
        <h1>ORGANIZA MT25 PRODUCCIONES</h1>
        <div class="redesMt25">
          <img src="~/static/logo.png">
          <div>
            <p>
              “NUESTROS DONES nos han sido dados junto con la encomienda de usarlos y desarrollarlos para la misión de la obra de Dios aquí en la tierra.“
            </p>
            <iframe
              id="facebookMT25"
              src="https://www.facebook.com/plugins/like.php?href=https%3A%2F%2Fwww.facebook.com%2Fministeriosmt25%2F&width=84&layout=button&action=like&size=small&share=false&height=65&appId"
              width="84"
              height="20"
              style="border:none;overflow:hidden"
              scrolling="no"
              frameborder="0"
              allowTransparency="true"
              allow="encrypted-media"
            ></iframe>
          </div>
        </div>
      </div>
      <div class="sigueBark">
        <h1>SIGUE A GRUPO BARAK</h1>
        <div class="redesBarak">
          <iframe
            id = "spotify"
            src="https://open.spotify.com/follow/1/?uri=spotify:artist:2IzxJqK9NbSIdw7rQVW03P?si=V0JgegMcQ8qYkz5SeZ1HCg&size=detail&theme=dark&show-count=0"
            width="300"
            height="56"
            scrolling="no"
            frameborder="0"
            style="border:none; overflow:hidden;"
            allowtransparency="true"
          ></iframe>
          <iframe
            id = "facebook"
            src="https://www.facebook.com/plugins/like.php?href=https%3A%2F%2Fwww.facebook.com%2FGrupoBarak%2F%3Fref%3Dbr_rs&width=100px&layout=button&action=like&size=small&height=65&appId"
            width="100%"
            height="65"
            style="border:none;overflow:hidden"
            scrolling="no"
            frameborder="0"
            allowTransparency="true"
            allow="encrypted-media"
          ></iframe>
        </div>
      </div>
    </div>
    <div class="final">
      <div class="terminos">
        <a href="#">TÉRMINOS Y CONDICIONES </a>
        <a href="#">CONTACTO DIRECTO </a>
        <a href="#">USO DE COOKIES </a>
      </div>
      <div>
        <div class="derechos">
          <div>
            <p>© 2020 TODOS LOS DERECHOS RESERVADOS. MT25PRODUCCIONES</p>
          </div>
        </div>
      </div>
      <br>
    </div>
  </div>
</template>

<style>
/* Ubicacion */
.ubicacion {
  z-index: -1;
  margin: 0 auto;
  height: 100vh;

}
.ubicacion .mapa{

  z-index: -1;
  margin: 0;
  width: 100%;
  height: 100vh;
 
}

/* video */
 #video {
  position: absolute;
  left: 0;
  top: -5%;
  width: 100%;
  height: 110%;
  z-index: -1;
  background-color: rgba(0,0,0,1);
}

/* terminos "*/
.final {
  justify-content: center;
  align-items: center;
  text-align: center;

  background-color: #2D2D2D;
}
.terminos {
  display:flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.terminos a {
  margin: 1vh;
  font-size: 10px;
  line-height: 12px;
  color: #FFFFFF;
  text-decoration:none;
  font-weight: 900;
}

.derechos {
  display:flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.derechos p {
  margin: 1vh;
  font-size: 10px;
  line-height: 12px;
  color: #FFFFFF;
  text-decoration:none;
  font-weight: 900;
}
/*Footer*/

.redesMt25 {
  display:flex;
  justify-content: left;
  align-items: left;
  text-align: left;
}
.redesMt25 p{
  margin: 1vh;
  font-size: 12px;
  line-height: 14px;
  justify-content: left;
  align-items: left;
  text-align: left;
}

#facebookMT25 {
  margin: 1vh;
}
.sigueMt5 img{
  margin: 1vh;
  width: auto;
  height: 100px;
  left: 180px;
  top: 2688px;
  grid-column-start: 1;
  grid-row-end: 3;
}
.sigueMt5 h1{
  font-weight: bold;
  font-size: 16px;
}

.sigueMt5{
  max-width: 50vh;
  margin: 3vh;
  margin-top: 6vh;
}
.sigueBark h1{
  font-weight: bold;
  font-size: 16px;
}

.redesBarak{
  display: grid;
  grid-template-columns:  60% 40%;
}

.sigueBark {
  max-width: 50vh;
  margin: 3vh;
  margin-top: 6vh;
}

#spotify {
  grid-column-start: 1;
  width: 50vh;

  margin: 5%;

}
#facebook {
  grid-column-start: 2;
  width: 40vh;
  margin-top: 20%;
  margin-left: 13%;
  /*
  margin: 3%;
  */
}

.footer {
  background-color: #2D2D2D;
  color: #fff;
  min-height: 30vh;
  line-height: 19px;
  display: flex;
  justify-content: center;
  align-items: flex-start;
  text-align: center;
}

/*entradas*/
.entradas {
  background-color: #2D2D2D;
  color: #fff;
  min-height: 70vh;
  line-height: 19px;
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

.entradas .reja {
  display: grid;
  grid-template-columns:  60vh 40vh;
  grid-template-rows: 5vh 25vh 5vh;
}
#zona1 {
   grid-column-start: 1;
   grid-row-start: 1;
   grid-row-end: 4;
}
#zona2 h1 {
  font-size: 28px;
  margin: 1vh;
}
#zona2 h4{
  font-size: 16px;
}
#zona2 {
   grid-column-start: 2;
   grid-row-start: 2;
   background: rgba(255, 255, 255, 0.75);
   margin-left: -10%;
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

  background: url('https://firebasestorage.googleapis.com/v0/b/diferentes-a2ca8.appspot.com/o/foto%20concierto%20anterior%20-%20bn.jpg?alt=media&token=0820554c-d11d-48ff-b9b3-44e2816c81ac');
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.descripcion h2{
  font-size: 36px;
}

/* invitados */
#invitados {
  z-index: 5;
  visibility: visible;
  background-color: #2D2D2D;
  min-height: 30vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
#invitados h3 {
  font-weight: 900;
  color: #fff;
  padding-bottom: 2px;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
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
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;

    background-color:  rgba(0, 39, 155, 0.25);
}

.title{
  display: block;
}
.title img{
  z-index: 100;
  visibility: visible;
  width: 30%;
}

.subtitle {
  z-index: 5;
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
  body {
    background-color: #2D2D2D;
  }
  /* Ubicacion */
  .ubicacion {
    z-index: -1;
    margin: 0 auto;
    height: 30vh;
  }
  .ubicacion .mapa{
    z-index: -1;
    margin: 0;
    width: 100%;
    height: 30vh;
  }
  /*video */
  #video{
    display:none;
  }
  /* terminos "*/
  .terminos {
    display:block;
  }

  /*Footer*/
  .redesMt25 {
    display:flex;
    justify-content: left;
    align-items: left;
    text-align: left;
  }
  .sigueMt5 img{
    margin: 1vh;
    grid-column-start: 1;
    grid-row-end: 3;
  }

  .sigueMt5{
    grid-row-start: 2;
    max-width: 50vh;
    margin: 3vh;
    margin-top: 3vh;
  }

  .redesBarak{
    display: grid;
    grid-template-columns:  60% 40%;
  }

  .sigueBark {
    grid-row-start: 1;
    max-width: 50vh;
    margin: 3vh;
    margin-top: 3vh;

  }
  #spotify {
    grid-column-start: 1;
    width: 40vh;

    margin: 5%;
  }
  #facebook {
    grid-column-start: 2;
    width: 15vh;
    margin-top: 20%;
    margin-left: 0%;
  }

  .footer {
    display: grid;
    grid-template-rows:  35% 30%;
  }
  /*entradas*/
  .entradas {
    min-height: 50vh;
    line-height: 19px;
  }
  .entradas h1 {
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 0px;
  }

  .entradas .reja {
    margin-top: 1vh;
    display: grid;
    grid-template-columns:  50% 50%;
    grid-template-rows:15vh ;
  }
  #zona1 {
    grid-column-start: 1;
    background-color: #2D2D2D;
    color: #fff;
  }
  #zona2 h1 {
    font-size: 18px;
    margin: 3vh;
  }
  #zona1 h1 {
    font-size: 18px;
  }
  #zona2 h4{
    font-size: 16px;
  }
  #zona2 {
    grid-column-start: 2;
    grid-row-start: 1;
    background-color: #2D2D2D;
    color: rgba(255, 255, 255, 0.75);
    background: rgba(0, 0, 0, 0);
  }
  /*descripcion*/
  .descripcion {
      background: url('https://firebasestorage.googleapis.com/v0/b/diferentes-a2ca8.appspot.com/o/foto%20concierto%20anterior%20-%20bn.jpg?alt=media&token=0820554c-d11d-48ff-b9b3-44e2816c81ac');
      /*esto es lo importate tamaño de imagen*/
      background-size: 100%;
      background-repeat: no-repeat;
      min-height: 35vh;
  }
  .descripcion h3{
    font-size: 12px;
  }
  .descripcion h2{
    font-size: 20px;
  }
  .descripcion p{
    font-size: 12px;
  }
  .espacios{
    display:none;
  }
  /* invitados */
  #invitados {
    min-height: 35vh;
  }
  #invitados h3 {
    font-weight: 900;
    color: #fff;
    margin-bottom: 1vh;
    font-weight: bold;
    font-size: 18px;
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
  .container {
    height: 60vh;
    background: url('https://firebasestorage.googleapis.com/v0/b/diferentes-a2ca8.appspot.com/o/fondo.png?alt=media&token=c7fedd12-091d-442d-8939-488c0f9dc083');
    background-position: center; /* Center the image */
    background-repeat: no-repeat; /* Do not repeat the image */
    background-size: cover; /* Resize the background image to cover the entire container */
 }

  .title img{
    width: 50%;
    padding-bottom: 10%;
    padding: 4vh;
  }
  .subtitle {
    display: none;
  }
  .fecha {
    font-weight: 900;
    font-size: 12px;
    color: #fff;
    padding-bottom: 2px;
  }
  .lugar {
    font-weight: 500;
    font-size: 12px;
    color: #fff;
    padding-bottom: 2px;
  }
}

</style>

<script>
import Navbar from '~/components/Navbar.vue'
import Card from '~/components/Card.vue'
import Boletos from '~/components/Boletos.vue'
import Mapa from '~/components/Mapa.vue'

export default {
  components: {
    Boletos,
    Navbar,
    Mapa,
    Card
  },
  data () {
    return {
      pantalla: '',
      comprar: ['COMPRAR ENTRADAS', 'COMPRAR']
    }
  },
  mounted () {
    this.pantalla = screen.width
  }
}
</script>
