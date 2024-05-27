<template>
    <div class="product-card">
      <img :src="product.image" alt="Shoe Image" />
      <div class="product-info">
        <h3>{{ product.name }}</h3>
        <p>{{ product.brand }}</p>
        <p>{{ product.price }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      product: Object,
    },
  };
  </script>
  
  <style scoped>
  .product-card {
    border: 1px solid #ccc;
    border-radius: 8px;
    overflow: hidden;
    text-align: center;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    max-width: 200px;
  }
  .product-card img {
    width: 100%;
    height: auto;
  }
  .product-info {
    padding: 1rem;
  }
  </style>
  