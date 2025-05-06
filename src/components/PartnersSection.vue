<template>
    <section id="partners" class="partners-section">
      <div class="container">
        <h2>Partner commerciali</h2>
        <p>Collaboriamo con aziende di riferimento nel settore per offrire soluzioni affidabili e innovative.</p>
        <div class="partner-logos">
          <!-- Loghi partner placeholder -->
          <div class="logo">Partner 1</div>
          <div class="logo">Partner 2</div>
          <div class="logo">Partner 3</div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  .partners-section {
    padding: 4rem 1rem;
    background-color: #ffffff;
    text-align: center;
  }
  
  .container {
    max-width: 960px;
    margin: 0 auto;
  }
  
  .partner-logos {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin-top: 2rem;
  }
  
  .logo {
    width: 120px;
    height: 60px;
    background-color: #e0e0e0;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: bold;
  }
  </style>
  