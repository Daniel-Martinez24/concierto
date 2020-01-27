<template>
  <div class="card">
    <div>
      <div class="ruedo">
        <h4> <strong>{{ numeroZona }} </strong></h4>
        <h4>{{ nombreZona }}</h4>
      </div>
      <h1>$400.00 MXN</h1>
      <el-button :type="typeBoton" round><strong>{{ textBoton }}</strong></el-button>
    </div>
  </div>
</template>

<script>
export default {
  props: [
    'numeroZona',
    'nombreZona',
    'tamaño',
    'typeBoton',
    'textBoton'
  ]
}
</script>

<style scoped>
.card{
    background-color: #fff;
    color:#2D2D2D;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    border-radius: 4px;
}
.card h1{
    margin: 3vh;
    font-size: 42px;
}
.ruedo{
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}
.ruedo h4{
    padding-left: 1vh;
    font-weight: 10;
}
</style>
