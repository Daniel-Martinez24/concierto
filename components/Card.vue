<template>
  <div id="card">
    <img src="https://imagenes.heraldo.es/files/image_990_v1/uploads/imagenes/2017/12/02/_mazin_eaa4ec1d.jpg" alt="">
    <div>
      <h3>{{ titulo }}</h3>
      <p>{{lugar}}</p>
    </div>
  </div>
</template>
<script>
export default {
  props: [
    'titulo',
    'lugar'
  ]
}
</script>

<style scoped>
#card {
   display: flex;
   align-items: center;
   text-align: center;
}
#card img {
    width: 10vh;
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
      width: 15vh;
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
