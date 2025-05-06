<template>
  <section id="services" class="services-section">
    <div class="wrapper">
      <h2>I nostri servizi</h2>

      <div class="service-block">
        <h3>Sviluppo su misura</h3>
        <p>
          Progettiamo software che si adatta perfettamente ai processi della tua azienda. Ogni soluzione è costruita partendo dalle reali esigenze operative, con l’obiettivo di semplificare il lavoro quotidiano e migliorare l’efficienza complessiva.
        </p>
      </div>

      <div class="service-block">
        <h3>Tecnologie moderne</h3>
        <p>
          Utilizziamo strumenti collaudati e aggiornati per costruire soluzioni robuste e durature: Express.js per gestire la logica applicativa, Vue.js per creare interfacce intuitive e dinamiche, e Sencha Ext JS per sviluppare portali complessi ad alte prestazioni. Ogni progetto nasce per integrarsi facilmente con le infrastrutture aziendali esistenti.
        </p>
      </div>

      <div class="service-block">
        <h3>Approccio consulenziale</h3>
        <p>
          Offriamo più di un servizio tecnico: affianchiamo ogni cliente come partner strategico. Analizziamo insieme obiettivi e criticità per definire soluzioni digitali concrete, sostenibili e realmente allineate con i processi aziendali.
        </p>
      </div>

      <div class="service-block">
        <h3>Assistenza e continuità</h3>
        <p>
          Restiamo al fianco dei nostri clienti anche dopo il rilascio. Forniamo supporto tecnico costante, manutenzione evolutiva e aggiornamenti funzionali per garantire nel tempo stabilità, sicurezza e adattabilità della soluzione.
        </p>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>

<style scoped lang="scss">
.services-section {
  padding: 6rem 0;
  background-color: #ffffff;
  text-align: left;

  .wrapper {
    max-width: 960px;
    margin: 0 auto;
    padding: 0 1rem;
  }

  h2 {
    font-size: 2.2rem;
    margin-bottom: 4rem;
    text-align: center;
  }

  .service-block {
    margin-bottom: 4rem;

    h3 {
      font-size: 1.4rem;
      color: #8b0000;
      margin-bottom: 1rem;
      text-align: center;
    }

    p {
      font-size: 1.1rem;
      line-height: 1.7;
      color: #333;
    }
  }
}
</style>
