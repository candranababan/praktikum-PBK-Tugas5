<template>
  <nav class="navbar">
    <div class="container">
      <a href="#" class="navbar-brand">my shoes store</a>
      <ul class="navbar-nav">
        <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Shop</a></li>
        <li class="nav-item"><a href="#" class="nav-link">Contact</a></li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  background-color: #333;
  color: #fff;
  padding: 1rem;
}
.navbar-brand {
  font-size: 1.5rem;
}
.navbar-nav {
  list-style: none;
  display: flex;
  gap: 1rem;
}
.nav-link {
  color: #fff;
  text-decoration: none;
}
.nav-link:hover {
  text-decoration: underline;
}
</style>
