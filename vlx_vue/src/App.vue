<template>
  <div>
    <SiteHeader @navigate="cambiaPercorso" />
    <component :is="componenteCorrente" />
  </div>
</template>

<script setup>
import { ref, computed, onMounted } from 'vue'
import SiteHeader from './components/SiteHeader.vue'
import HomePage from './views/HomePage.vue'
import ChiSiamoPage from './views/ChiSiamoPage.vue'
import ContattiPage from './views/ContattiPage.vue'

const percorso = ref(window.location.pathname)

onMounted(() => {
  window.addEventListener('popstate', () => {
    percorso.value = window.location.pathname
  })
})

// Mappa dei percorsi
const mappa = {
  '/': HomePage,
  '/chi-siamo': ChiSiamoPage,
  '/contatti': ContattiPage
}

const componenteCorrente = computed(() => mappa[percorso.value] || HomePage)

function cambiaPercorso(nuovoPercorso) {
  if (nuovoPercorso !== percorso.value) {
    window.history.pushState({}, '', nuovoPercorso)
    percorso.value = nuovoPercorso
  }
}
</script>

<style scoped>
</style>
