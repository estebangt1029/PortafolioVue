<script setup>
   import MenuCom from '../components/MenuCom.vue';
   import RedesCom from '../components/RedesCom.vue';
</script>

<template>
    <MenuCom></MenuCom>
    <RedesCom></RedesCom>
    <main>
        <section class="about-section">
            <div class="container">
                <h2 class="section-title"><span class="var">Var </span><span class="variable">¡Hola!</span>;</h2>
                <h3 class="section-subtitle"><span class="var">Let </span><span class="variable">Soy</span>=<span class="llaves">[</span><span class="string">'Esteban','Moreno'</span><span class="llaves">]</span>;</h3>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Soy un entusiasta desarrollador full stack con un enfoque especializado en front-end. A lo largo de mi trayectoria, he invertido tiempo y esfuerzo en proyectos personales apasionantes, así como en colaboraciones ocasionales con equipos.<span class="p">{{'</p>'}}</span></p>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Mi experiencia se basa en proyectos personales donde he tenido la oportunidad de desarrollar aplicaciones web desde cero. Estos proyectos han sido una valiosa oportunidad para perfeccionar mis habilidades en HTML, CSS y JavaScript, y también me han permitido explorar diferentes frameworks y bibliotecas como Vue.js. y Laravel<span class="p">{{'</p>'}}</span></p>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Además de mis proyectos personales, he tenido el privilegio de colaborar con equipos de desarrollo. Estas colaboraciones me han brindado una visión más amplia del proceso de trabajo en equipo y me han permitido aprender de otros profesionales del campo. Estas experiencias han sido un valioso complemento para mi desarrollo como desarrollador full stack.<span class="p">{{'</p>'}}</span></p>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Aunque mi experiencia puede parecer más limitada en términos de colaboraciones formales, mi pasión y dedicación hacia el front-end son evidentes en mis proyectos personales. Me apasiona la creación de interfaces atractivas y la búsqueda de soluciones creativas para mejorar la experiencia del usuario.<span class="p">{{'</p>'}}</span></p>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Mi portafolio muestra una selección de mis proyectos personales y colaboraciones, destacando mi enfoque en el front-end y mi capacidad para llevar a cabo implementaciones limpias y efectivas.<span class="p">{{'</p>'}}</span></p>

                <p class="section-description"><span class="p">{{'<p>'}}</span>Si estás buscando un desarrollador full stack con una sólida base en front-end y la voluntad de enfrentar nuevos desafíos, estaré encantado de colaborar contigo en tu próximo proyecto. Juntos, podemos convertir ideas en realidad y crear experiencias web memorables.<span class="p">{{'</p>'}}</span></p>
            </div>
        </section>

    </main>
    
</template>

<style scoped>

main{
    width: 100vw;
    min-height: 100vh;
    background-color: black;
  
}
.p{
    color: red;
}
.var{
    color: blueviolet;
}
.variable{
    color: rgb(0, 129, 129);
}
.llaves{
    color: rgb(255, 238, 1);
}
.string{
    color: chartreuse;
}
.about-section {
  padding: 60px 35px;
}

.container {
  max-width: 800px;
  margin: 0 auto;
}

.section-title {
  font-size: 32px;
  font-weight: bold;
  color: white;
  margin-bottom: 20px;
}

.section-subtitle {
  font-size: 24px;
  font-weight: bold;
  color: white;
  margin-bottom: 10px;
}

.section-description {
  font-size: 16px;
  line-height: 1.6;
  color: #dfdfdf;
  margin-bottom: 15px;
}

</style>
