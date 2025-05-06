<template>
  <section id="about" class="about-section">
    <div class="container">
      <h2>Chi siamo</h2>
      <p>
        Con oltre 30 anni di esperienza, Veleex è un punto di riferimento nello sviluppo di soluzioni software su misura per aziende che vogliono affrontare la trasformazione digitale con solidità e visione.
        Progettiamo portali, applicazioni e sistemi gestionali perfettamente integrati con i processi aziendali, mettendo al centro affidabilità, scalabilità e supporto costante.
        Collaboriamo fianco a fianco con ogni cliente per costruire strumenti realmente utili, orientati all’efficienza e pensati per durare nel tempo.
      </p>

      <div class="cards">
        <div class="card">
          <div class="icon-title">
            <h3>➤ Affidabilità</h3>
          </div>
          <p>Soluzioni stabili e testate, pensate per garantire continuità operativa in ogni contesto aziendale.</p>
        </div>
        <div class="card">
          <div class="icon-title">
            <h3>➤ Su misura</h3>
          </div>
          <p>Ogni progetto è modellato sulle esigenze specifiche del cliente, senza soluzioni preconfezionate.</p>
        </div>
        <div class="card">
          <div class="icon-title">
            <h3>➤ Esperienza</h3>
          </div>
          <p>Oltre tre decenni di lavoro con imprese in settori diversi: un patrimonio di competenze sempre aggiornato.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
.about-section {
  padding: 6rem 1rem;
  background-color: #f4f4f4;
  text-align: left;

  .container {
    max-width: 960px;
    margin: 0 auto;
  }

  h2 {
    font-size: 2.2rem;
    margin-bottom: 2rem;
  }

  p {
    font-size: 1.2rem;
    line-height: 1.8;
  }

  .cards {
    margin-top: 4rem;
    display: flex;
    flex-direction: column;
    gap: 3rem;

    @media (min-width: 768px) {
      flex-direction: row;
    }

    .card {
      flex: 1;
      padding: 2rem;
      background-color: #f4f4f4;
      text-align: left;
      position: relative;

      &::before {
        content: "";
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
        width: 4px;
        height: 140px;
        background-color: #8b0000;
        transition: all 0.3s ease;
      }

      &:hover::before {
        height: 80%;
        top: 10%;
        transform: none;
      }

      .icon-title h3 {
        font-size: 1.5rem;
        color: #8b0000;
        margin-bottom: 1rem;
        display: flex;
        align-items: center;
        gap: 0.5rem;
      }

      p {
        font-size: 1.1rem;
        line-height: 1.6;
      }
    }
  }
}
</style>
