<script setup>
import DatosPersonales from './components/icons/DatosPersonales.vue';
import NavBar from './components/icons/NavBar.vue';
</script>

<template>
  <header>
  <!---  Barra de navecacion--->
  <NavBar/>
  <!---  Datos personales--->
  <DatosPersonales/>
  </header>
  <main>
    <section id="educacion">
      <h2>Educación - Cursos</h2>
    </section>
    <section id="experiencia">
      <h2>Experiencia</h2>
    </section>
    <section id="proyectos">
      <h2>Proyectos</h2>
    </section>
    <section id="habilidades">
      <h2>Habilidades</h2>
    </section>
    <section id="intereses">
      <h2>intereses</h2>
    </section>
  </main>
</template>

<style scoped>

</style>
