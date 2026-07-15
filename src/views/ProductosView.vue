<script setup>
import EncabezadoApp from '../components/EncabezadoApp.vue'
import { ref } from 'vue'

const emit = defineEmits(['cambiarVista'])

const productos = ref([
  { id: 1, nombre: 'Pan de Batalla', precio: 0.50, stock: 100 },
  { id: 2, nombre: 'Cuñapé', precio: 2.00, stock: 50 },
  { id: 3, nombre: 'Empanada de Queso', precio: 3.50, stock: 30 }
])

function volverInicio() {
  emit('cambiarVista', 'inicio')
}
</script>

<template>
  <div class="vista-productos">

    <EncabezadoApp 
      titulo="Gestión de Productos" 
      subtitulo="Administra el inventario de la panadería"
    />

    <main class="contenedor-productos">

      <button class="btn-volver" @click="volverInicio">
        ← Volver al inicio
      </button>

      <h2>Lista de Productos</h2>

      <table class="tabla-productos">

        <thead>
          <tr>
            <th>ID</th>
            <th>Producto</th>
            <th>Precio (Bs.)</th>
            <th>Stock</th>
          </tr>
        </thead>

        <tbody>
          <tr v-for="prod in productos" :key="prod.id">
            <td>{{ prod.id }}</td>
            <td>{{ prod.nombre }}</td>
            <td>{{ prod.precio.toFixed(2) }}</td>
            <td>{{ prod.stock }} u.</td>
          </tr>
        </tbody>

      </table>

    </main>

  </div>
</template>

<style scoped>

.contenedor-productos {
  max-width: 800px;
  margin: 30px auto;
  padding: 20px;
  background: white;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0,0,0,.1);
}

.btn-volver {
  background: #92400e;
  color: white;
  border: none;
  padding: 10px 18px;
  border-radius: 6px;
  cursor: pointer;
  margin-bottom: 20px;
}

.btn-volver:hover {
  background: #d97706;
}

.tabla-productos {
  width: 100%;
  border-collapse: collapse;
  margin-top: 15px;
}

.tabla-productos th,
.tabla-productos td {
  border: 1px solid #ddd;
  padding: 12px;
  text-align: left;
}

.tabla-productos th {
  background-color: #f4f6f9;
  color: #92400e;
}

</style>
