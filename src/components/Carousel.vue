<template>
    <div class="carousel">
      <div class="carousel-item" v-for="(image, index) in images" :key="index">
        <img :src="image" alt="Shoe Collection" />
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        images: [
          'images/sneakers1.jpeg',
          'images/sneakers2.jpg',
          'images/sneakers3.jpg',
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .carousel {
    display: flex;
    overflow-x: auto;
    gap: 1rem;
  }
  .carousel-item {
    min-width: 100%;
  }
  .carousel-item img {
    width: 100%;
    height: auto;
  }
  </style>
  