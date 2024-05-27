<template>
  <div id="app">
    <Navbar />
    <Carousel />
    <div class="products">
      <ProductCard v-for="product in products" :key="product.id" :product="product" />
    </div>
    <Footer />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Carousel from './components/Carousel.vue';
import ProductCard from './components/ProductCard.vue';
import Footer from './components/Footer.vue';

export default {
  components: {
    Navbar,
    Carousel,
    ProductCard,
    Footer,
  },
  data() {
    return {
      products: [
        { id: 1, name: 'Nike Air Max', brand: 'Nike', price: 'Rp 550.000', image: 'images/nikeairmax.jpg' },
        { id: 2, name: 'Adidas Ultra Boost', brand: 'Adidas', price: 'Rp 750.000', image: 'images/adidas.jpg' },
        { id: 3, name: 'Puma RS-X', brand: 'Puma', price: 'Rp 800.000', image: 'images/puma rs-x.jpg' },
        { id: 4, name: 'Reebok Classic', brand: 'Reebok', price: 'Rp 450.000', image: 'images/rebook.jpg' },
        { id: 5, name: 'New Balance 574', brand: 'New Balance', price: 'Rp 600.000', image: 'images/new balence.jpg' },
      ],
    };
  },
};
</script>

<style>
.products {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  padding: 2rem;
  justify-content: center;
}
</style>
