<template>
  <div id="card">
    <img v-if="imagen == 'primera'" src="~/static/levantandoaltareslogo.jpg" alt="">
    <img v-else src="~/static/foto-perfil-barak.jpg" alt="">
    <div>
      <h3>{{ titulo }}</h3>
      <p>{{lugar}}</p>
    </div>
  </div>
</template>
<script>
export default {
  props: [
    'imagen',
    'titulo',
    'lugar'
  ],
  data () {
    return {
      foto: '~/static/levantandoaltareslogo.jpg'
    }
  }
}
</script>

<style scoped>
#card {
   display: flex;
   align-items: center;
   text-align: center;
}
#card img {
    width: 56.84px;
    height: 56.78px;
    left: 1.26px;
    top: 1.89px;
    border-radius: 50px;
    margin-right: 2vh;
    border-width: 2px;
    border-style: solid;
    border-color: #fff;
}
#card p {
    color: #828282;
   align-items: left;
   text-align: left;
}
#card h3 {
  font-weight: 300;
  font-size: 18px;
  color: #fff;
  padding-bottom: 2px;
}

@media (max-width: 600px){
  #card img {
      width: 56.84px;
      height: 56.78px;
      border-style: solid;
      border-color: #fff;
  }
  #card p {
    align-items: left;
    text-align: left;
  }
  #card h3 {
    font-weight: 300;
    font-size: 16px;
    color: #fff;
    padding-bottom: 2px;
  }
}
</style>
