<template>
  <section id="services" class="services-section">
    <div class="wrapper">
      <h2>I nostri servizi</h2>

      <div class="service-block">
        <div class="service-content reverse">
          <img src="/images/icons/icon_1.png" alt="Icona Sviluppo su misura" />
          <div class="text">
            <h3>Sviluppo su misura</h3>
            <p>
              Progettiamo software che si adatta perfettamente ai processi della tua azienda.
              Ogni soluzione è costruita partendo dalle reali esigenze operative, con l’obiettivo
              di semplificare il lavoro quotidiano e migliorare l’efficienza complessiva.
            </p>
          </div>
        </div>
      </div>

      <div class="service-block">
        <div class="service-content">
          <img src="/images/icons/icon_2.png" alt="Icona Tecnologie moderne" />
          <div class="text">
            <h3>Tecnologie moderne</h3>
            <p>
              Utilizziamo strumenti collaudati e aggiornati per costruire soluzioni robuste e
              durature: Express.js per gestire la logica applicativa, Vue.js per creare interfacce
              intuitive e dinamiche, e Sencha Ext JS per sviluppare portali complessi ad alte
              prestazioni. Ogni progetto nasce per integrarsi facilmente con le infrastrutture
              aziendali esistenti.
            </p>
          </div>
        </div>
      </div>

      <div class="service-block">
        <div class="service-content reverse">
          <img src="/images/icons/icon_3.png" alt="Icona Approccio consulenziale" />
          <div class="text">
            <h3>Approccio consulenziale</h3>
            <p>
              Offriamo più di un servizio tecnico: affianchiamo ogni cliente come partner
              strategico. Analizziamo insieme obiettivi e criticità per definire soluzioni digitali
              concrete, sostenibili e realmente allineate con i processi aziendali.
            </p>
          </div>
        </div>
      </div>

      <div class="service-block">
        <div class="service-content">
          <img src="/images/icons/icon_4.png" alt="Icona Assistenza e continuità" />
          <div class="text">
            <h3>Assistenza e continuità</h3>
            <p>
              Restiamo al fianco dei nostri clienti anche dopo il rilascio. Forniamo supporto
              tecnico costante, manutenzione evolutiva e aggiornamenti funzionali per garantire nel
              tempo stabilità, sicurezza e adattabilità della soluzione.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<style scoped lang="scss">
.services-section {
  padding: 6rem 0;
  background-color: #ffffff;

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
  }

  .service-content {
    display: flex;
    align-items: center;
    gap: 2rem;
    margin-bottom: 3rem;

    img {
      width: 250px;
      height: 250px;
      flex-shrink: 0;
    }

    .text {
      flex: 1;

      h3 {
        font-size: 1.4rem;
        color: #1a1a1a;
        margin-bottom: 1rem;
      }

      p {
        font-size: 1.1rem;
        line-height: 1.7;
        color: #333;
      }
    }

    &.reverse {
      flex-direction: row-reverse;

      .text {
        text-align: left;
      }
    }
  }

  @media (max-width: 768px) {
      .service-content {
        flex-direction: column !important;
        gap: 1rem;
        margin-bottom: 2rem;
        align-items: flex-start;
        align-items: center;

        img {
          width: 100%;
          height: auto;
          max-width: 200px;
        }

        .text {
          text-align: left;
        }
      }

      .service-block {
        margin-bottom: 2rem;
      }
    }
}
</style>
