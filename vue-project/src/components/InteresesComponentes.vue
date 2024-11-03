<script>
import Fondolava from './Fondolava.vue'; // Importa el nuevo componente

export default {
  components: {
    Fondolava // Registra el componente
  },
  data() {
    return {
      intereses: [
        'Inglés : Domino el inglés a nivel avanzado, lo que me permite acceder a recursos y conectarme globalmente. Mi habilidad de lectura y comunicación en inglés refuerza mis conocimientos técnicos y amplía mis oportunidades profesionales.',

        'Libros: La lectura me inspira y fomenta el pensamiento crítico. Mis géneros preferidos (ciencia ficción, historia y tecnología) enriquecen mi visión, permitiéndome aplicar ideas innovadoras y compartir recomendaciones para promover el amor por los libros.',

        'Tecnología: La tecnología es una herramienta esencial en mi vida profesional. Me mantengo actualizado en temas como programación e inteligencia artificial, aplicándolos en proyectos y explorando su impacto ético para un futuro responsable.'
      ]
    }
  }
}
</script>

<template>
  <div class="intereses-contenedor">
    <!-- Fondo animado dentro del contenedor -->
    <Fondolava /> <!-- Utiliza el componente importado -->

    <!-- Lista de intereses -->
    <ul class="contenedor-lista">
      <li v-for="(interes, index) in intereses" :key="index" class="item">
        {{ interes }}
      </li>
    </ul>
  </div>
</template>

<style scoped>
/* Contenedor principal de intereses */
.intereses-contenedor {
  position: relative;
  width: 100%; /* Asegura que ocupe el 100% de su contenedor padre */
  max-width: 100%; /* Ajusta el ancho máximo para que sea el 100% */
  margin: 2rem auto; /* Centrado con margen superior e inferior */
  padding: 2rem; /* Ajusta el padding para un diseño más limpio */
  border-radius: 10px; /* Esquinas redondeadas */
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2); /* Sombra sutil */
}

/* Fondo animado */
.fondo-animado {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -1; /* Asegura que el fondo esté detrás del contenido */
}

/* Lista de intereses */
.contenedor-lista {
  list-style-type: none; /* Sin viñetas */
  padding: 0; /* Sin padding en la lista */
  margin: 0; /* Sin margen en la lista */
  color: rgb(255, 255, 255); /* Color de texto */
  font-size: 1.4rem; /* Tamaño de fuente */
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8); /* Sombra de texto sutil */
}

.item {
  margin-bottom: 1rem; /* Espaciado entre elementos */
  line-height: 1.5; /* Mejora la legibilidad */
}
</style>