<template>
  <main>
    <main_JumboTron />
    <main_devsCourses
    :courses="courses"
    />
    <main_bg_banner />
    <main_recent_courses
    :recent_courses_menu="recent_courses_menu"
    :courses="courses"
    :side_menu_icons="side_menu_icons"
    />
    <main_newsLetter />
    <main_popsCourses
    :courses="courses"
    />
    <main_noStudentsAction/>
    <main_testimonial/>
  </main>
</template>

<script>
import main_JumboTron from './main_JumboTron.vue'
import main_devsCourses from './main_devsCourses.vue'
import main_bg_banner from './main_bg_banner.vue'
import main_recent_courses from './main_recent_courses.vue'
import main_newsLetter from './main_newsLetter.vue'
import main_popsCourses from './main_popsCourses.vue'
import main_noStudentsAction from './main_noStudentsAction.vue'
import main_testimonial from './main_testimonial.vue'

export default {
  name: 'MainPage',
  components: {
    main_JumboTron,
    main_devsCourses,
    main_bg_banner,
    main_recent_courses,
    main_newsLetter,
    main_popsCourses,
    main_noStudentsAction,
    main_testimonial
  },
  props: ['courses', 'recent_courses_menu', 'side_menu_icons'],
}
</script>

<style lang="scss" scoped>
</style>