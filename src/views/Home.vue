<script setup>
   import MenuCom from '../components/MenuCom.vue';
   import RedesCom from '../components/RedesCom.vue';
</script>

<template>
  <div class="container1">
    <!-- components -->
    <MenuCom></MenuCom>
    <RedesCom></RedesCom>
    <!-- 1 -->
    <div class="content">
      <!-- <h1>I AM <span>Esteban Moreno</span></h1> -->
      <div class="content2">
        <div class="visible">
          <p>I AM :</p> 
          <ul>
            <li>Esteban</li>
            <li>18 Years</li>
            <li>Full Stack</li>
          </ul>  
        </div>
      </div>
    
      <div class="foto">
        <img class="foto" src="../assets/yo.jpg" alt="">
        <div class="skils">
          <img class="img1" src="../assets/icons8-css3-48.png" alt="">
          <img class="img2" src="../assets/icons8-html-5-48.png" alt="">
          <img class="img3" src="../assets/icons8-javascript-48.png" alt="">
          <img class="img4" src="../assets/icons8-mariadb-48.png" alt="">
          <img class="img5" src="../assets/icons8-postgresql-48.png" alt="">
          <img class="img6" src="../assets/icons8-vue-js-48.png" alt="">
          <img class="img7" src="../assets/icons8-laravel-48.png" alt="">
          <img class="img8" src="../assets/icons8-oreja-48.png" alt="">
          <!-- <img class="img9" src="../assets/icons8-mongodb-48.png" alt=""> -->
        </div>
      </div>
      <div class="info">
        <p>Soy Esteban Moreno, un desarrollador Full Stack con experiencia en el desarrollo de aplicaciones web modernas.
        Mi enfoque principal es el desarrollo frontend, utilizando tecnologías como HTML, CSS y JavaScript, junto con frameworks como Vue.js y Bootstrap.
        Además, tengo experiencia en el desarrollo de aplicaciones backend utilizando el framework Laravel y trabajando con bases de datos como MariaDB, PostgreSQL y MongoDB.</p>
      </div>
    </div>
    <!-- 2 -->
    <h2>Certificados</h2>
    <div class="certificados">
      <a href="https://www.sololearn.com/certificates/CC-PXLBYEWM"><img class="certificado" src="../assets/JS.jpg" alt=""></a>
      <a href="https://www.sololearn.com/certificates/CC-AJUXU0HX"><img class="certificado" src="../assets/CSS.jpg" alt=""></a>  
      <a href="https://www.sololearn.com/certificates/CT-YFKZ4FAR"><img class="certificado" src="../assets/HTML.png" alt=""></a>
    </div>
    <!-- 3 -->
    <h2>Projects</h2>
    <div class="projects">
      <a href="#"><img class="project" src="https://res.cloudinary.com/daqs7crna/image/upload/v1685313433/Captura_desde_2023-05-28_17-36-36_vafdum.png" alt=""></a>
      <a href="#"><img class="project" src="https://res.cloudinary.com/daqs7crna/image/upload/v1685314224/Captura_desde_2023-05-28_17-50-09_iqnylm.png" alt=""></a>
      <a href="#"><img class="project" src="https://res.cloudinary.com/daqs7crna/image/upload/v1685315948/Captura_desde_2023-05-28_18-18-52_yqohba.png" alt=""></a>
    </div>
  </div>
</template>
<style scoped>


.container1{
  min-height: 100vh;
  max-width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: 'Creepster', cursive;
  background: rgb(0,0,0);
  background: linear-gradient(180deg, rgba(0,0,0,1) 0%, rgba(0,0,0,1) 41%, rgba(231,76,60,1) 100%, rgba(231,76,60,1) 100%);
  padding-bottom: 50px;
 
}
 
  .content{
    max-width: 100vw;
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: space-around;
    gap: 40px;
    flex-wrap: wrap;
    
  }
  .foto{
    width: 250px;
    border-radius: 50%;
    display: flex;
  }
  h1{
    color: #fff;
    text-align: center;
  }
  h2{
    color: white;
    text-align: center;
  }
  .info{
    width: 33%;
    color: #fff;
    text-align: center;
    display: flex;
    flex-direction: column;
    gap: 5px;
  }

  .certificados{
    max-width: 90vw;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    gap: 10px;
  }
  .certificado{
    width: 350px;
  }

  .projects{
    max-width: 90vw;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    gap: 10px;
  }
  .project{
    width: 350px;
  }
  




/* animacion del texto */
.content2 {
  font-size:36px;
  line-height:40px;
  font-family:'Muli';
  color:#ecf0f1;
  height:40px;
  width: 33%;
  text-align: center;
  position: relative;
  padding-left: 40px;
}

.content2:before {
    content:'{';
    position:absolute;
    left: 5px;
    line-height:40px;
  }
  .content2:after {
    content:'}';
    position:absolute;
    right: 5px;
    line-height:40px;
  }
  .content2:after, .content2:before {
    color:#e74c3c;
    font-size:42px;
    animation:4s linear 0s normal none infinite opacity;
    -webkit-animation:4s ease-out 0s normal none infinite opacity;
    -moz-animation:4s ease-out 0s normal none infinite opacity;
    -o-animation:4s ease-out 0s normal none infinite opacity;
  }


.visible {
  float:left;
  font-weight:600;
  overflow:hidden;
  height:40px;   
}

p {
  display:inline;
  float:left;
  margin:0;
}

ul {
  margin-top:0;
  padding-left:110px;
  text-align:left;
  list-style:none;
  animation:9s linear 0s normal none infinite change;
  -webkit-animation:9s linear 0s normal none infinite change;
  -moz-animation:9s linear 0s normal none infinite change;
  -o-animation:9s linear 0s normal none infinite change;
}
ul:hover{
  animation-play-state: paused;
}

ul li {
  line-height:40px;
  margin:0;
}


@keyframes opacity {
  0%   {opacity:0;}
  50%  {opacity:1;}
  100% {opacity:0;}
}

@keyframes change {
  0%   {margin-top:0;}
  15%  {margin-top:0;}
  25%  {margin-top:-40px;}
  40%  {margin-top:-40px;}
  50%  {margin-top:-80px;}
  65%  {margin-top:-80px;}
  75%  {margin-top:-40px;}
  85%  {margin-top:-40px;}
  100% {margin-top:0;}
}






  /* animacion de tecnologias rotando*/
  .skils{
    position: absolute;
    width: 250px;
    height: 250px;
    animation-name: rotar;
    animation-duration: 25s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
  }
  .skils:hover{
    animation-play-state: paused;
  }
  .img1{
    rotate: -45deg;
    position: absolute;
    left: 0px;
    top: 0px;

  }
  .img2{
    position: absolute;
    right: 0;
    rotate: 45deg;
    right: 0px;
    top: 0px;
  }
  .img3{
    position: absolute;
    bottom: 0px;
    left: 0px;
    rotate: -135deg;
  }
  .img4{
    position: absolute;
    bottom: 0px;
    right: 0px;
    rotate: 135deg;
  }
  .img5{
    position: absolute;
    bottom: 40%;
    left: -45px;
    rotate: -90deg;
  }
  .img6{
    position: absolute;
    bottom: 40%;
    right: -45px;
    rotate: 90deg;
  }
  .img7{
    position: absolute;
    bottom: -45px;
    left: 40%;
    rotate: 180deg;
  }
  .img8{
    position: absolute;
    top: -45px;
    left: 40%;
  }
/* 
  @keyframes rotar {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  } */







  @media only screen and (max-width: 600px) {
  
  .container1{
    padding-top: 40px;
  }
  .info{
    width: 95%;
  }
  .content2 {
  font-size:36px;
  line-height:40px;
  font-family:'Muli';
  color:#ecf0f1;
  height:40px;
  width: 100%;
  text-align: center;
  position: relative;
  padding-left: 40px;
}
}


</style>