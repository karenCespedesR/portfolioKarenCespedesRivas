<script setup>
import DatosPersonales from './components/DatosPersonales.vue';
import NavBar from './components/NavBar.vue';
import Educacion from './components/EducacionComponentes.vue';
import ExperienciaComponente from './components/ExperienciaComponentes.vue';
import ProyectosComponentes from './components/ProyectosComponentes.vue';
import HabilidadesComponentes from './components/HabilidadesComponentes.vue';
import InteresesComponentes from './components/InteresesComponentes.vue';
</script>

<template>
  <header>
  <!---  Barra de navecacion--->
  <NavBar/>
  <!---  Datos personales--->
  <DatosPersonales/>
  </header>
  <main>
      <section id="educacion" class="seccion">
         <h2>Educación</h2>
         <Educacion />
      </section>
      <section id="experiencia" class="seccion">
         <h2>Experiencia</h2>
         <ExperienciaComponente />
      </section>
      <section id="proyectos" class="seccion">
         <h2>Proyectos</h2>
         <ProyectosComponentes />
      </section>
      <section id="habilidades" class="seccion">
         <h2>Habilidades</h2>
         <HabilidadesComponentes />
      </section>
      <section id="intereses" class="seccion">
         <h2>Intereses</h2>
         <InteresesComponentes />
      </section>
   </main>
   <footer class="footer">
      <a href="#top">Inicio</a>
      <p>2024 Karen Céspedes Rivas - Portafolio Web</p>
   </footer>
</template>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Montserrat', sans-serif; /* Cambiar a Montserrat */
    color: #960069; /* Azul Profundo */
    background-color: #fae0f6; /* Azul Muy Claro */
    margin: 0;
}

h2 {
    font-size: 1.8rem;
    font-weight: 700;
    margin-bottom: 1rem;
    color: #d102a4; /* Azul Real */
    text-transform: uppercase;
    letter-spacing: 0.1em;
    border-bottom: 2px solid #fcb3f2; /* Azul Gris Claro */
    padding-bottom: 0.5rem;
}

.seccion {
    padding: 3rem 0;
    width: 90%; /* Aumentar el ancho para dispositivos pequeños */
    max-width: 800px;
    margin: 0 auto;
}

.footer {
    width: 100%; /* Para asegurarnos de que ocupe toda la ventana */
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
    font-size: 1.2rem;
    background-color: #eba0e1; /* Azul Cielo */
    color: #960082; /* Azul Profundo */
}

.footer a {
    color: #960082; /* Azul Profundo */
    text-decoration: none;
    font-weight: bold;
    margin-bottom: 0.5rem;
}

.footer p {
    font-size: 0.9rem;
}

/* Media Queries para Responsividad */
@media (max-width: 768px) {
    h2 {
        font-size: 1.5rem; /* Ajustar el tamaño de fuente del encabezado */
        text-align: center; /* Centrar el texto */
    }
    .seccion {
        padding: 2rem 0; /* Reducir el padding en dispositivos más pequeños */
    }
}

@media (max-width: 480px) {
    h2 {
        font-size: 1.3rem; /* Ajustar aún más el tamaño de fuente del encabezado */
        text-align: center; /* Centrar el texto en pantallas aún más pequeñas */
    }
    .footer {
        font-size: 1rem; /* Reducir el tamaño de fuente del pie de página */
    }
}
</style>
