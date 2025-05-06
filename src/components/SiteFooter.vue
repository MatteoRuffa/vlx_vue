<template>
    <footer class="site-footer">
      <div class="container">
        <p>&copy; 2025 Nome Azienda. Tutti i diritti riservati.</p>
        <div class="social-links">
          <a href="#">LinkedIn</a>
          <a href="#">GitHub</a>
          <a href="#">Email</a>
        </div>
      </div>
    </footer>
  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  .site-footer {
    background-color: #f8f8f8;
    padding: 2rem 1rem;
    text-align: center;
    border-top: 1px solid #ddd;
  }
  
  .container {
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .social-links {
    margin-top: 1rem;
    display: flex;
    justify-content: center;
    gap: 1.5rem;
  }
  
  .social-links a {
    text-decoration: none;
    color: #333;
  }
  </style>
  