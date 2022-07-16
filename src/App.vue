<!-- Creare un progetto con Vue CLI, strutturando il layout in almeno 3 macro-componenti:
HeaderPage, MainPage e FooterPage.

Suddivisione FooterPage in 2 e HeaderPage in 3 micro-componenti
Suddivisione MainPage in 7/8 micro-componenti o sections

Popolare le voci di menù di HeaderPage e FooterPage dinamicamente, tramite delle props, creando una struttura dati idonea.
Aggiungere in App.vue i data che riporto con props alle componenti discendenti

Preparo in assets le immagini e i colori a cui dare dei nomi più specifici in base a quali componenti o sections verranno usati
importo bootstrap -->

<template>
  <div id="app">
    <HeaderPage
    :links="links"
    :social_links="social_links"
    :nav_menu_links="nav_menu_links"
    />
  </div>
</template>

<script>
import nav_menu_links from './assets/nav_menu_links.json'
import HeaderPage from './components/HeaderPage.vue'
export default {
  name: 'App',
  components: {
    HeaderPage,
  },
  data() {
    return {
      links: ['Home', 'Pages', 'Course Formats', 'Courses', 'Demos'],
      social_links: ['fa-facebook', 'fa-twitter', 'fa-instagram', 'fa-linkedin', 'fa-google-plus', 'fa-youtube'],
      nav_menu_links: nav_menu_links
    }
  }
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';
</style>