<template>
  <div class="bg-gray-800 text-white rounded-lg p-6 border-2 border-purple-500 shadow-lg shadow-purple-500/50 hover:shadow-lg hover:shadow-purple-500/70 transition-all duration-300">
    <h2 class="text-2xl font-bold mb-4">{{ title }}</h2>
    <p class="text-gray-300">{{ content }}</p>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  content: String,
});
</script>

<style scoped>
/* Fondo oscuro para la tarjeta */
div {
  background-color: #2d2d2d; /* Fondo gris oscuro */
  border-radius: 12px;
  transition: all 0.3s ease;
  border-color: #9b4dca; /* Borde morado siempre visible */
  box-shadow: 0 4px 20px rgba(155, 77, 202, 0.6); /* Sombra morada sutil siempre visible */
}

/* Sombra más intensa al hacer hover sobre la tarjeta */
div:hover {
  box-shadow: 0 4px 30px rgba(155, 77, 202, 0.8); /* Sombra morada más intensa al pasar el ratón */
}
</style>
