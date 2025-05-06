<template>
  <header class="site-header" :class="{ open: isMenuOpen }">
    <div class="container">
      <div class="logo">
        <img src="/logo.png" alt="Veleex Logo" />
        <span class="logo-text">Veleex</span>
      </div>
      <nav class="menu-desktop">
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">Chi siamo</a></li>
          <li><a href="#services">Servizi</a></li>
          <li><a href="#partners">Partners</a></li>
        </ul>
      </nav>
      <button class="hamburger" @click="toggleMenu">
        <span></span>
        <span></span>
        <span></span>
      </button>
    </div>

    <div class="menu-mobile" v-if="isMenuOpen">
      <button class="close" @click="toggleMenu">&times;</button>
      <ul>
        <li><a href="#home" @click="toggleMenu">Home</a></li>
        <li><a href="#about" @click="toggleMenu">Chi siamo</a></li>
        <li><a href="#service" @click="toggleMenu">Servizi</a></li>
        <li><a href="#partners" @click="toggleMenu">Partners</a></li>
      </ul>
    </div>
  </header>
</template>

<script setup>
import { ref } from 'vue'
const isMenuOpen = ref(false)
const toggleMenu = () => (isMenuOpen.value = !isMenuOpen.value)
</script>

<style scoped lang="scss">
.site-header {
  position: fixed;
  top: 0;
  width: 100%;
  background-color: #fff;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  z-index: 1000;

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .logo img {
    height: 40px;
  }

  .menu-desktop {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);

    ul {
      display: flex;
      gap: 4rem;
      list-style: none;
      margin: 0;
      padding: 0;

      li {
        position: relative;

        a {
          text-decoration: none;
          color: #333;
          font-weight: 500;
          display: inline-block;
          padding-bottom: 5px;
          transition: transform 0.2s ease;

          &::after {
            content: "";
            position: absolute;
            left: 0;
            bottom: 0;
            width: 0;
            height: 2px;
            background-color: #8b0000;
            transition: width 0.3s ease;
          }

          &:hover {
            transform: scale(1.05);

            &::after {
              width: 100%;
            }
          }
        }
      }
    }
  }

  .hamburger {
    display: none;
    flex-direction: column;
    gap: 4px;
    background: none;
    border: none;
    cursor: pointer;

    span {
      width: 25px;
      height: 3px;
      background: #333;
    }
  }

  .menu-mobile {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #fff;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    z-index: 9999;

    ul {
      list-style: none;
      text-align: center;

      li {
        margin: 1.5rem 0;
        position: relative;

        a {
          font-size: 2rem;
          color: #333;
          text-decoration: none;
          font-weight: 500;
          padding-bottom: 5px;
          transition: transform 0.2s ease;

          &::after {
            content: "";
            position: absolute;
            left: 0;
            bottom: 0;
            width: 0;
            height: 2px;
            background-color: #8b0000;
            transition: width 0.3s ease;
          }

          &:hover {
            transform: scale(1.05);

            &::after {
              width: 100%;
            }
          }
        }
      }
    }

    .close {
      position: absolute;
      top: 1.5rem;
      right: 2rem;
      background: none;
      border: none;
      font-size: 2rem;
      cursor: pointer;
    }
  }

  @media (max-width: 768px) {
    .menu-desktop {
      display: none;
    }

    .hamburger {
      display: flex;
    }
  }
}
</style>
