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
    <HeaderPage :links="links" :social_links="social_links" :nav_menu_links="nav_menu_links" />
    <MainPage :courses="courses" :recent_courses_menu="recent_courses_menu" :side_menu_icons="side_menu_icons" />
  </div>
</template>

<script>
import nav_menu_links from './assets/nav_menu_links.json'
import { links, social_links, courses, recent_courses_menu, side_menu_icons } from './assets/data.js'


import HeaderPage from './components/HeaderPage.vue'
import MainPage from './components/MainPage.vue'

export default {
  name: 'App',
  components: {
    HeaderPage,
    MainPage,
  },
  data() {
    return {
      links: links,
      social_links: social_links,
      nav_menu_links: nav_menu_links,
      courses: courses,
      recent_courses_menu: recent_courses_menu,
      side_menu_icons: side_menu_icons,
    }
  }
}
</script>

<style lang="scss">
@import './assets/scss/style.scss';
</style>