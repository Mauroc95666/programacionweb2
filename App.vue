<template>
  <main>
    <h1>Mi contenido reutilizable</h1>

    <Card
      titulo="Producto 1"
      descripcion="Esta es una tarjeta reutilizable en Vue."
    />

    <Card
      titulo="Producto 2"
      descripcion="Puedo cambiar los datos sin crear otro componente."
    />
  </main>
</template>

<script setup>
import Card from './components/Card.vue'
</script>