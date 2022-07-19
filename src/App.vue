<!-- Creare un progetto con Vue CLI, strutturando il layout in almeno 3 macro-componenti:
HeaderPage, MainPage e FooterPage.

Suddivisione FooterPage in 2 e HeaderPage in 3 micro-componenti + i componenti per menu dinamici
Suddivisione MainPage in 7/8 micro-componenti o sections + componenti per menu dinamici

Popolare le voci di menù di HeaderPage e FooterPage dinamicamente, tramite delle props, creando una struttura dati idonea.

Aggiungere in App.vue i data che riporto con props alle componenti discendenti

Preparo in assets le immagini e i colori e i file data

importo bootstrap
importo il font e fontawesome per icone -->

<template>
  <div id="app">
    <HeaderPage :links="links" :social_links="social_links" :nav_menu_links="nav_menu_links" />
    <MainPage :courses="courses" :recent_courses_menu="recent_courses_menu" :side_menu_icons="side_menu_icons" />
    <FooterPage :footer_socials="footer_socials"/>

  </div>
</template>

<script>
import nav_menu_links from './assets/nav_menu_links.json'
import { links, social_links, courses, recent_courses_menu, side_menu_icons, footer_socials } from './assets/data.js'


import HeaderPage from './components/HeaderPage.vue'
import MainPage from './components/MainPage.vue'
import FooterPage from './components/FooterPage.vue'

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage,
    FooterPage,
  },
  data() {
    return {
      links: links,
      social_links: social_links,
      nav_menu_links: nav_menu_links,
      courses: courses,
      recent_courses_menu: recent_courses_menu,
      side_menu_icons: side_menu_icons,
      footer_socials: footer_socials,
    }
  }
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';
</style>