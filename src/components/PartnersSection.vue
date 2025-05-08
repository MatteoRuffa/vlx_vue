<template>
  <section id="partners" class="partners-section">
    <div class="wrapper">
      <h2>I nostri partner</h2>
      <p class="description">
        Collaboriamo con aziende affidabili e innovative che condividono i nostri valori e ci aiutano a offrire soluzioni di qualità su misura per ogni cliente.
      </p>
      <div class="partners-grid">
        <div class="partner-logo">
          <img src="/images/patners/acrolcar.jpg" alt="Partner 1" />
        </div>
        <div class="partner-logo">
          <img src="/images/patners/crf.png" alt="Partner 2" />
        </div>
        <div class="partner-logo">
          <img src="/images/patners/goma.png" alt="Partner 3" />
        </div>
        <div class="partner-logo">
          <img src="/images/patners/renaudo.png" alt="Partner 4" />
        </div>
      </div>
      <div class="bando-logo">
        <a href="/TARGA-MANIFESTO.pdf" target="_blank" rel="noopener">
          <img src="/logo_bando_1.jpg" alt="Logo Bando" />
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
.partners-section {
  padding: 4rem 0;
  background-color: #f9f9f9;
  text-align: center;

  .wrapper {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 1rem;
  }

  h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
  }

  .description {
    font-size: 1.1rem;
    color: #555;
    margin-bottom: 3rem;
    max-width: 800px;
    margin-left: auto;
    margin-right: auto;
    padding:  2rem;
  }

  .partners-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 3rem;
    padding: 2rem 0;
  }

  .partner-logo {
    flex: 1 1 200px;
    max-width: 200px;
  }

  .partner-logo img {
    width: 100%;
    height: auto;
    object-fit: contain;
  }

  .bando-logo {
  margin-top: 3rem;
  display: flex;
  justify-content: center;
  padding: 2rem;

  img {
    width: 40vw;
    max-width: 100%;
    height: auto;
    object-fit: contain;
  }

  @media (max-width: 768px) {
    img {
      width: 90vw;
    }
  }
}


}
</style>
