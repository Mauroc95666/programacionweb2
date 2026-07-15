<script setup>
defineProps({
  titulo: {
    type: String,
    required: true
  },
  subtitulo: {
    type: String,
    required: true
  },
  adicional: {
    type: String,
    required: false,
    default: ''
  }
})
</script>

<template>
  <header class="encabezado">
    <h1>{{ titulo }}</h1>
    <p class="subtitulo">{{ subtitulo }}</p>
    <span v-if="adicional" class="adicional">{{ adicional }}</span>
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
  font-size: 2rem;
}

.subtitulo {
  margin: 8px 0 0;
  font-size: 1.1rem;
  opacity: 0.9;
}

.adicional {
  display: block;
  margin-top: 8px;
  font-size: 0.9rem;
  color: #d97706; /* Tono ámbar que combina con la interfaz de la panadería */
  font-weight: 500;
  letter-spacing: 0.5px;
}
</style>
