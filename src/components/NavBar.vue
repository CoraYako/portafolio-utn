<template>
  <nav class="navbar">
    <div class="navbar-menu">
      <ul>
        <a v-for="item in navegacion" :key="item.nombre" :href="item.enlace" class="nav-item">{{ item.nombre }}</a>
      </ul>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';
const navegacion = ref([
  { id: 1, nombre: 'educacion', enlace: 'Educación' },
  { id: 2, nombre: 'experiencia', enlace: 'Experiencia' },
  { id: 3, nombre: 'proyectos', enlace: 'Proyectos' },
  { id: 4, nombre: 'habilidades', enlace: 'Habilidades' },
]);
</script>

<style scoped>
.navbar {
  background-color: var(--vt-c-indigo);
  color: #fff;
  padding: 0.5rem 1rem;
  align-items: center;
}

.navbar-item {
  color: #fff;
  text-decoration: none;
  margin-right: 1rem;
}

.navbar-menu {
  display: flex;
  justify-content: flex-end;
}

.nav-list {
  list-style: none;
}

a {
  border: 1px solid;
  border-color: hsla(160, 100%, 37%, 0.2);
  border-radius: 5px;
  /* Elimina la subrayado de los enlaces y elementos con clase "green" */
  text-decoration: none;
  /* Añade una transición suave para los cambios de estilo */
  transition: 0.4s;
  /* Añade padding alrededor del contenido */
  padding: 5px;
}

a:hover {
  /* Cambia el color de fondo al pasar el mouse sobre un enlace */
  background-color: hsla(160, 100%, 37%, 0.2);
}

@media (max-width: 768px) {
  .navbar-menu {
    display: flex;
    justify-content: flex-end;
    width: 100%;
  }
}
</style>
