<template>
  <div id="navBar" class="text">
    <ul id="izquiera">
      <li id="imagen">
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
      right: 2vh;
  }
  #derecha li{
      float:left;
      align-items: center;
  }
  #derecha li p{
      color: white;
      font-weight: 900;
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
      margin-top: 3.5vh;

      margin-left: -15%;
      color: #00279B;
      display: flex;
      justify-content: center;
      align-items: center;
      font-weight: 800;
  }
  #irMain p {
      display: flex;
      justify-content: center;
      align-items: center;
      margin: -4%;
  }
  @media (max-width: 600px){
    #izquiera li img{
        display: none;
    }
    #navBar ul li{
        margin: 1vh;
    }
    #izquiera li{
        margin: 0vh;
    }
    #navBar{
        top: 0%;
    }
    #irMain {
        height: 1vh;
        width: 90%;
        margin-top: 0vh;

        margin-left: 0%;
        display: flex;
    }
    #irMain p {
        margin: -4%;
        Font-Size: 10px;
    }
    #derecha li p{
        Font-Size: 12px;
    }
  }
</style>
