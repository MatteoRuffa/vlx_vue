<template>
  <section id="home" class="hero-section">
    <div class="background"></div>
    <div class="content">
      <h1>Tecnologia e precisione al servizio delle imprese.</h1>
      <p>Progettiamo software e portali gestionali per semplificare, innovare e far crescere il tuo business.</p>
      <button>Contattaci ora</button>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
.hero-section {
  position: relative;
  width: 100%;
  min-height: 60vh;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding-left: 5%;
  padding-top: 15%;
  background-color: #fff;
  overflow: hidden;

  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-image: url('@/assets/hero.png');
    background-size: cover;
    background-position: center;
    opacity: 0.4;
    z-index: 1;
  }

  .content {
    position: relative;
    z-index: 2;
    max-width: 700px;

    h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
    }

    button {
      background-color: #8b0000;
      color: #fff;
      padding: 0.75rem 1.5rem;
      border: none;
      font-size: 1rem;
      cursor: pointer;
      transition: background-color 0.3s;

      &:hover {
        background-color: #a00000;
      }
    }
  }
}
</style>