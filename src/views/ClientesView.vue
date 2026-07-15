<script setup>
import EncabezadoApp from '../components/EncabezadoApp.vue'

const emit = defineEmits(['cambiarVista'])

function volverInicio() {
  emit('cambiarVista', 'inicio')
}
</script>

<template>
  <div class="vista-clientes">

    <EncabezadoApp
      titulo="Gestión de Clientes"
      subtitulo="Administración de clientes de la panadería"
    />

    <main class="contenedor-clientes">

      <h2>Lista de Clientes</h2>

      <p>
        Aquí podrás registrar y consultar los clientes.
      </p>

      <button @click="volverInicio">
        ← Volver al inicio
      </button>

    </main>

  </div>
</template>


<style scoped>

.contenedor-clientes {
  max-width:800px;
  margin:30px auto;
  padding:30px;
  background:white;
  border-radius:10px;
  text-align:center;
  box-shadow:0 2px 10px rgba(0,0,0,.1);
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

button:hover {
  background:#92400e;
}

</style>
