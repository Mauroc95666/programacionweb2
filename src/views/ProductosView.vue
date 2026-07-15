<script setup>
import EncabezadoApp from '../components/EncabezadoApp.vue'
import { ref } from 'vue'

// Lista de productos de prueba
const productos = ref([
  { id: 1, nombre: 'Pan de Batalla', precio: 0.50, stock: 100 },
  { id: 2, nombre: 'Cuñapé', precio: 2.00, stock: 50 },
  { id: 3, nombre: 'Empanada de Queso', precio: 3.50, stock: 30 }
])
</script>

<template>
  <div class="vista-productos">
    <!-- Reutilizamos el encabezado en esta nueva pantalla -->
    <EncabezadoApp 
      titulo="Gestión de Productos" 
      subtitulo="Administra el inventario de la panadería"
      adicional="Sección de Inventario"
    />

    <main class="contenedor-productos">
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
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.tabla-productos {
  width: 100%;
  border-collapse: collapse;
  margin-top: 15px;
}

.tabla-productos th, .tabla-productos td {
  border: 1px solid #ddd;
  padding: 12px;
  text-align: left;
}

.tabla-productos th {
  background-color: #f4f6f9;
  color: #92400e;
}
</style>
