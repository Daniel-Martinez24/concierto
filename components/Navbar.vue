<template>
  <div id="navBar" class="text">
    <ul id="izquiera">
      <li><el-button id="irMain" round><p>MT25 PRODUCCIONES</p></el-button></li>
    </ul>
    <ul id="derecha">
      <li><el-button type="text">ACCEDE A TU CUENTA</el-button></li>
    </ul>
  </div>
</template>

<style scoped>
  #irMain {
      height: 1vh;
      width: 100%;
      margin: -10%;
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
  }
</style>
