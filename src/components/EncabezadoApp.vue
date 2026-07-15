<script setup>
defineProps({
  titulo: {
    type: String,
    required: true
  },
  subtitulo: {
    type: String,
    required: true
  }
})
</script>

<template>
  <header class="encabezado">
    <h1>{{ titulo }}</h1>
    <p>{{ subtitulo }}</p>
  </header>
</template>

<style scoped>
.encabezado {
  padding: 24px;
  background-color: #1a1717;
  color: white;
  text-align: center;
}

.encabezado h1 {
  margin: 0;
}

.encabezado p {
  margin: 8px 0 0;
}
</style>

