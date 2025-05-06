<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-logo">
        <img src="/src/assets/logo-footer.png" alt="Logo Veleex Srl" />
      </div>
      <div class="footer-info">
        <p class="company-name">Veleex Srl</p>
        <p>Via Esempio 123, 00100 Roma</p>
        <p>P.IVA 12345678901</p>
        <p>info@veleex.it</p>
      </div>
      <div class="footer-links">
        <ul>
          <li><a href="#">Chi siamo</a></li>
          <li><a href="#">Servizi</a></li>
          <li><a href="#">Partner</a></li>
          <li><a href="#">Contatti</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <p>© 2025 Veleex Srl - Tutti i diritti riservati.</p>
    </div>
  </footer>
</template>

<script setup>
</script>

<style scoped lang="scss">
.footer {
  background-color: #1a1a1a;
  color: #f0f0f0;
  padding: 3rem 1rem 1rem;

  .footer-content {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    max-width: 1200px;
    margin: 0 auto;
    gap: 2rem;

    .footer-logo {
      flex: 1 1 200px;

      img {
        width: 100%;
        max-width: 150px;
        height: auto;
        object-fit: contain;
      }
    }

    .footer-info {
      flex: 1 1 300px;
      font-size: 0.95rem;

      .company-name {
        font-weight: bold;
        margin-bottom: 0.5rem;
      }

      p {
        margin: 0.3rem 0;
      }
    }

    .footer-links {
      flex: 1 1 200px;

      ul {
        list-style: none;
        padding: 0;

        li {
          margin: 0.5rem 0;

          a {
            color: #f0f0f0;
            text-decoration: none;
            transition: color 0.3s;

            &:hover {
              color: #d32f2f;
            }
          }
        }
      }
    }
  }

  .footer-bottom {
    text-align: center;
    margin-top: 2rem;
    font-size: 0.85rem;
    border-top: 1px solid #333;
    padding-top: 1rem;
    color: #aaa;
  }
}
</style>
