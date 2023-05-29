<script setup>
   import ProjectsCom from '../components/ProjectsCom.vue';
   import MenuCom from '../components/MenuCom.vue';
   
   const projects = [
     {
       image: 'https://res.cloudinary.com/daqs7crna/image/upload/v1685313433/Captura_desde_2023-05-28_17-36-36_vafdum.png',
       title: 'Portafolio Personal',
       description: 'Mi portafolio personal es un proyecto que he desarrollado para mostrar mis habilidades y experiencia en el campo del desarrollo web.Este mismo portafolio que estás viendo es una representación de mi trabajo y una muestra de mis capacidades en diseño y programación.En este portafolio, he utilizado tecnologías como HTML, CSS y JavaScript para crear una interfaz moderna y atractiva. Además, he implementado el framework Vue.js para mejorar la interactividad y la experiencia del usuario.Mi objetivo al crear este portafolio es presentar mi habilidad para desarrollar aplicaciones web de alta calidad, demostrar mi capacidad para trabajar con diferentes tecnologías y frameworks, y ofrecer una visión general de mis logros y conocimientos en el campo del desarrollo.Estoy entusiasmado por compartir mi trabajo contigo y espero que este portafolio sea una muestra sólida de mis habilidades y mi dedicación al mundo del desarrollo web.',
       repo:'https://icons.getbootstrap.com/icons/info-circle-fill/'
     },
     {
       image: 'https://res.cloudinary.com/daqs7crna/image/upload/v1685314224/Captura_desde_2023-05-28_17-50-09_iqnylm.png',
       title: 'Cronological Task Manager',
       description: 'Es un proyecto que he desarrollado utilizando Laravel Jetstream y Vue Inertia. Se trata de un administrador de tareas que te permite organizar y gestionar tus actividades de manera cronológica y eficiente.Con esta aplicación, podrás crear, editar y eliminar tareas, asignarles fechas de vencimiento y prioridades, así como marcarlas como completadas una vez que se hayan finalizado.Utilizando Laravel Jetstream como framework de backend, he implementado un sistema de autenticación seguro que te permite registrarte, iniciar sesión y mantener tus tareas privadas y protegidas. Por otro lado, Vue Inertia se encarga de la parte del frontend, brindando una experiencia de usuario fluida y dinámica sin necesidad de recargar la página.Cronological Task Manager es un proyecto que demuestra mi habilidad para trabajar con Laravel Jetstream y Vue Inertia, así como mi capacidad para desarrollar aplicaciones web funcionales y eficientes.'
     },
     {
       image: 'https://res.cloudinary.com/daqs7crna/image/upload/v1685315948/Captura_desde_2023-05-28_18-18-52_yqohba.png',
       title: 'Juego de Memoria',
       description: 'Es un proyecto que he desarrollado utilizando HTML, CSS y JavaScript.En este juego, se presentan varias cartas boca abajo y el objetivo es encontrar las parejas de cartas que coincidan. Cada vez que selecciones dos cartas, se voltearán y si coinciden, se mantendrán descubiertas. De lo contrario, volverán a su posición inicial y deberás recordar su ubicación para futuros intentos.He diseñado una interfaz atractiva y fácil de usar utilizando HTML y CSS para crear las cartas y darle estilo al tablero de juego. Además, he utilizado JavaScript para implementar la lógica del juego, como el seguimiento de las cartas seleccionadas, la validación de las coincidencias y el recuento de los intentos realizados.El Juego de Memoria es una muestra de mi habilidad para crear aplicaciones interactivas utilizando tecnologías web fundamentales. He enfatizado en la experiencia del usuario, proporcionando animaciones suaves, efectos visuales y una retroalimentación clara para hacer del juego una experiencia divertida y entretenida.A través de este proyecto, he puesto en práctica mis habilidades en diseño web, programación y lógica para crear una experiencia envolvente y desafiante.¡Te invito a probar el Juego de Memoria y disfrutar de un momento de diversión mientras ejercitas tu memoria y habilidades de concentración!'
     },
     {
       image: 'https://res.cloudinary.com/daqs7crna/image/upload/v1683298712/Captura_desde_2023-05-05_09-57-29_ydxaz6.png',
       title: 'Clon del Login de Instagram',
       description: 'El Clon del Login de Instagram es un proyecto en el que me he enfocado en recrear la interfaz de inicio de sesión de la popular aplicación Instagram utilizando tecnologías web como HTML, CSS.En este proyecto, me he centrado en replicar fielmente la apariencia y el diseño del formulario de inicio de sesión de Instagram. He utilizado HTML para estructurar los elementos del formulario y CSS para aplicar estilos y dar formato a los distintos componentes, como campos de texto, botones y fondos.Este clon del login de Instagram es un ejemplo de mi habilidad para recrear interfaces de usuario de manera precisa y detallada. A través de este proyecto, he demostrado mi conocimiento en diseño web, manipulación de estilos con CSS.Este proyecto es una muestra de mi capacidad para trabajar en la parte visual de aplicaciones web, brindando una experiencia atractiva y familiar a los usuarios.'
     }
   ];
</script>

<template>
    <MenuCom></MenuCom>
    <div class="container">
       <ProjectsCom v-for="(project, index) in projects" :key="index" :image="project.image" :title="project.title" :description="project.description"></ProjectsCom>
    </div>
</template>

<style scoped>
    .container{
        width: 100vw;
        min-height: 100vh;
        padding-top: 10vh;
        padding-bottom: 5vh;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        background-color: black;
        color: white;
        gap: 20px;
    }

</style>
