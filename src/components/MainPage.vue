<template>
  <main>
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
    <main_testimonial_banner/>
  </main>
</template>

<script>
import main_devsCourses from './main_devsCourses.vue'
import main_bg_banner from './main_bg_banner.vue'
import main_recent_courses from './main_recent_courses.vue'
import main_newsLetter from './main_newsLetter.vue'
import main_popsCourses from './main_popsCourses.vue'
import main_noStudentsAction from './main_noStudentsAction.vue'
import main_testimonial_banner from './main_testimonial_banner.vue'

export default {
  name: 'MainPage',
  components: {
    main_devsCourses,
    main_bg_banner,
    main_recent_courses,
    main_newsLetter,
    main_popsCourses,
    main_noStudentsAction,
    main_testimonial_banner
  },
  props: ['courses', 'recent_courses_menu', 'side_menu_icons'],
}
</script>

<style lang="scss" scoped>
</style>