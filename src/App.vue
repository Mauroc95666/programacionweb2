<script setup>
import { ref } from 'vue' // <-- codigo luis: Importamos ref para controlar la vista activa
import InicioView from './views/InicioView.vue'
import ProductosView from './views/ProductosView.vue' // <-- codigo luis: Importamos tu vista de productos

// codigo luis: Estado para saber qué pantalla mostrar
const vistaActiva = ref('inicio')

// codigo luis: Detecta si se hace clic en la tarjeta de Productos dentro de InicioView
const manejarClicInicio = (event) => {
  const tarjeta = event.target.closest('.tarjeta')
  if (tarjeta && tarjeta.textContent.includes('Productos')) {
    vistaActiva.value = 'productos'
  }
}
// fin codigo luis
</script>

<template>
  <div class="app">
    <!-- codigo luis: Renderizado condicional de las pantallas -->
    <!-- Si la vista es productos, mostramos tu componente -->
    <ProductosView v-if="vistaActiva === 'productos'" />

    <!-- Si es inicio, mostramos el componente de tu compañero y escuchamos sus clics -->
    <div v-else @click="manejarClicInicio">
      <InicioView />
    </div>

    <!-- Botón flotante para volver atrás cuando estés en Productos -->
    <button 
      v-if="vistaActiva !== 'inicio'" 
      @click="vistaActiva = 'inicio'" 
      class="boton-volver"
    >
      ⬅ Volver al Inicio
    </button>
    <!-- fin codigo luis -->
  </div>
</template>

<style scoped>
.app {
  min-height: 100vh;
  background-color: #f4f6f9;
}

/* codigo luis: Estilo para el botón flotante de volver */
.boton-volver {
  position: fixed;
  bottom: 20px;
  right: 20px;
  padding: 12px 20px;
  background-color: #1a1717;
  color: white;
  border: none;
  border-radius: 8px;
  cursor: pointer;
  font-weight: bold;
  box-shadow: 0 4px 10px rgba(0,0,0,0.2);
  z-index: 100;
}
.boton-volver:hover {
  background-color: #d97706;
}
/* fin codigo luis */
</style>
