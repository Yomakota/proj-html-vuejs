<template>
  <main>
    <main_JumboTron />
    <main_devsCourses :courses="courses" />
  </main>
</template>

<script>
import main_JumboTron from './main_JumboTron.vue'
import main_devsCourses from './main_devsCourses.vue'

export default {
  name: 'MainPage',
  components: {
    main_JumboTron,
    main_devsCourses,
  },
    props:['courses'],
}
</script>

<style lang="scss" scoped>
</style>