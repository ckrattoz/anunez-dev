<template>
  <div class="app-container">
    <h1 class="main-title neon-text">Antonio N.</h1>
    <div class="posts-container">
      <PostCard
          v-for="(post, index) in posts"
          :key="index"
          :title="post.title"
          :content="post.content"
      />
    </div>
  </div>
</template>

<script setup>
import PostCard from './PostCard.vue';

const posts = [
  { title: 'Introduction to Programming', content: 'Learn the basics of programming and how to get started with any programming language.' },
  { title: 'Understanding Variables', content: 'Variables are used to store data. In programming, a variable is a container for data values.' },
  { title: 'Loops and Control Flow', content: 'Loops help you execute a block of code multiple times. Control flow determines the order in which code is executed.' },
  { title: 'Functions and Methods', content: 'Functions are blocks of code that perform a specific task. Methods are functions associated with an object.' },
];
</script>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background: #0f0f0f; /* Fondo oscuro */
  background-image: radial-gradient(circle, rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 0.9)); /* Efecto de niebla blanca */
  padding: 20px;
  overflow: hidden; /* Para evitar barras de desplazamiento innecesarias */
}

.main-title {
  font-size: 4rem;
  font-weight: bold;
  color: #9b4dca; /* Morado brillante */
  text-align: center;
  margin-bottom: 30px;
  font-family: 'Orbitron', sans-serif; /* Fuente futurista */
  letter-spacing: 5px;
  text-shadow: 0 0 10px rgba(155, 77, 202, 0.8), 0 0 20px rgba(155, 77, 202, 0.8), 0 0 30px rgba(155, 77, 202, 0.8);
  animation: neon 1.5s ease-in-out infinite alternate;
}

/* Animación de neón para el título */
@keyframes neon {
  0% {
    text-shadow: 0 0 10px rgba(155, 77, 202, 0.8), 0 0 20px rgba(155, 77, 202, 0.8), 0 0 30px rgba(155, 77, 202, 0.8);
  }
  100% {
    text-shadow: 0 0 20px rgba(155, 77, 202, 1), 0 0 40px rgba(155, 77, 202, 1), 0 0 60px rgba(155, 77, 202, 1);
  }
}

.posts-container {
  display: flex;
  flex-direction: column; /* Asegura que las tarjetas estén en una columna */
  gap: 20px; /* Espaciado entre las tarjetas */
  width: 100%;
  max-width: 600px; /* Puedes ajustar este ancho máximo */
  margin-top: 20px;
  padding-bottom: 20px; /* Para no cortar las tarjetas al hacer scroll */
}
</style>
