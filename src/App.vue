<script setup>
import NavBar from './components/NavBar.vue'
import DatosPersonales from './components/DatosPersonales.vue'
import EducacionYCursos from './components/EducacionYCursos.vue'
import Experiencia from './components/ExperienciaProfesional.vue'
import ProyectosVarios from './components/ProyectosVarios.vue'
import HabilidadesVarias from './components/HabilidadesVarias.vue'
</script>

<template>
  <header>
    <NavBar />
    <DatosPersonales />
  </header>
  <main>
    <section id="educacion">
      <h2>Educación - Cursos</h2>
      <EducacionYCursos />
    </section>
    <section id="experiencia">
      <h2>Experiencia</h2>
      <Experiencia />
    </section>
    <section id="proyectos">
      <h2>Proyectos</h2>
      <ProyectosVarios />
    </section>
    <section id="habilidades">
      <h2>Habilidades</h2>
      <HabilidadesVarias />
    </section>
    <section id="intereses">
      <h2>Intereses</h2>
    </section>
  </main>
</template>

<style scoped></style>
