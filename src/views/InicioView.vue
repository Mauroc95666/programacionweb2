<script setup>
import EncabezadoApp from '../components/EncabezadoApp.vue'
</script>

<template>
  <div class="app">
    <EncabezadoApp
      titulo="Panadería Kiataque"
      subtitulo="Sistema de Gestión de Inventario y Ventas"
    />

    <main class="contenedor-panaderia">
      <section class="panel-bienvenida">
        <h2>¡Bienvenido al Panel de Control!</h2>

        <p>
          Desde aquí podrás administrar toda la información de la panadería de
          forma rápida y sencilla.
        </p>

        <div class="opciones">
          <div class="tarjeta">
            <h3>🍞 Productos</h3>
            <p>Registrar, editar y consultar los productos disponibles.</p>
          </div>

          <div class="tarjeta">
            <h3>👥 Clientes</h3>
            <p>Administrar la información de los clientes registrados.</p>
          </div>

          <div class="tarjeta">
            <h3>🛒 Ventas</h3>
            <p>Controlar pedidos, ventas diarias y facturación.</p>
          </div>
        </div>
      </section>
    </main>
  </div>
</template>

<style scoped>
.app {
  min-height: 100vh;
  background-color: #f4f6f9;
}

.contenedor-panaderia {
  max-width: 1000px;
  margin: 30px auto;
  padding: 20px;
}

.panel-bienvenida {
  background: white;
  padding: 30px;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.panel-bienvenida h2 {
  color: #d97706;
  margin-bottom: 15px;
}

.panel-bienvenida p {
  color: #555;
  line-height: 1.6;
}

.opciones {
  margin-top: 30px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 20px;
}

.tarjeta {
  background: #fff8e1;
  border-left: 5px solid #d97706;
  border-radius: 8px;
  padding: 20px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.tarjeta:hover {
  transform: translateY(-5px);
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
}

.tarjeta h3 {
  margin-bottom: 10px;
  color: #92400e;
}

.tarjeta p {
  color: #555;
}
</style>
