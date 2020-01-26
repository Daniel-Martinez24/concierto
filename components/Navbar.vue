<template>
  <div id="navBar" class="text">
    <ul id="izquiera">
      <li>
        <el-button type="text">
          <img src="~/static/logo.png" alt="">
        </el-button>
      </li>
      <li><el-button id="irMain" round><p>MT25 PRODUCCIONES</p></el-button></li>
    </ul>
    <ul id="derecha">
      <li>
        <el-button type="text">
          <p>
            ACCEDE A TU CUENTA
          </p>
        </el-button>
      </li>
    </ul>
  </div>
</template>

<style scoped>
  .text {
      Font-Family: fantasy;
      Font-Style: Bold;
      Font-Size: 14px;
  }
  #navBar{
      background-color: (0, 0, 0, 0);
      width: 100%;
      height: 10%;
      top: 1%;
      left: 0;
      position: fixed;

      display: flex;
      align-items: center;
  }
  #navBar ul{
      display: inline-block;
  }
  #navBar ul li{
      display: inline-block;
      margin: 3vh;
  }
  #derecha {
      float: right;
      position: absolute;
      margin-left: 80%;
  }
  #derecha li{
      float:left;
      align-items: center;
  }
  #derecha li p{
      color: white;
  }
  #izquiera {
      margin: 0%;
      padding: 0%;
  }
  #izquiera li {
      float:left;
      align-items: center;
  }
  #izquiera li img{
      height: 7vh;
      width: 7vh;
      margin: 0%;
      padding: 0%;
  }
  #irMain {
      height: 1vh;
      width: auto;
      margin-top: 11%;

      margin-left: -15%;
      color: #00279B;
      display: flex;
      justify-content: center;
      align-items: center;
  }
  #irMain p {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: -4%;
  }
</style>
