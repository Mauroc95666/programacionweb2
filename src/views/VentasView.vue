<script setup>
import EncabezadoApp from '../components/EncabezadoApp.vue'

const emit = defineEmits(['cambiarVista'])

function volverInicio() {
  emit('cambiarVista', 'inicio')
}
</script>

<template>
  <div>
    <EncabezadoApp
      titulo="Gestión de Ventas"
      subtitulo="Control de pedidos y ventas de la panadería"
    />

    <main class="pagina">
      <h2>Ventas</h2>

      <p>
        Aquí podrás registrar y consultar las ventas realizadas.
      </p>

      <button @click="volverInicio">
        ← Volver al inicio
      </button>
    </main>
  </div>
</template>

<style scoped>
.pagina {
  max-width: 800px;
  margin: 30px auto;
  padding: 30px;
  background:white;
  border-radius:10px;
  text-align:center;
}

button {
  margin-top:20px;
  padding:10px 20px;
  background:#d97706;
  color:white;
  border:none;
  border-radius:6px;
  cursor:pointer;
}
</style>
