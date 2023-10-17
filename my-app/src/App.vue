<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div>
    <header>
      <div class="wrapper">
        <nav>
          <RouterLink to="/" class="nav-link">Home</RouterLink>
          <RouterLink to="/about" class="nav-link">About</RouterLink>
        </nav>
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
  background-color: #000; 
  padding: 1rem;
}

.wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

nav {
  display: flex;
  gap: 1rem;
}

.nav-link {
  text-decoration: none;
  color: #fff; 
  padding: 0.5rem 1rem;
  border: 1px solid #fff; 
  border-radius: 4px;
  transition: background-color 0.3s;
}

.nav-link:hover {
  background-color: #fff; 
  color: #000; 
}

@media (min-width: 1024px) {
  header {
    padding: 2rem;
  }
}
</style>
