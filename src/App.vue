<script setup></script>

<template>
  


  <main class="contenedor-panaderia">
    <header>
      <h1>Panadería Kiataque</h1>
      <p class="subtitulo">Sistema de Gestión de Inventario y Ventas</p>
    </header>

    <section class="panel-bienvenida">
      <h2>¡Bienvenido al Panel de Control!</h2>
      <p>Desde aquí podrás administrar los productos, clientes y órdenes del día.</p>
    </section>
  </main>

</template>

<style scoped>

.contenedor-panaderia {
  max-width: 800px;
  margin: 40px auto;
  padding: 20px;
  background-color: #ffffff;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.subtitulo {
  text-align: center;
  color: #6b7280;
  font-style: italic;
}

.panel-bienvenida {
  margin-top: 30px;
  padding: 20px;
  border-left: 5px solid #d97706;
  background-color: #fffbeb;
}
</style>
