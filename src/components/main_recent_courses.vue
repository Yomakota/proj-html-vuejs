<template>
        <div class="container-fluid position-relative my-5">
            <div class="row justify-content-center">
                <div class="col-11 text-center">
                    <h1>Recent courses</h1>
                    <ul class="row row-cols-8 list-unstyled justify-content-center my-5">
                        <li v-for="element, index in recent_courses_menu" :key="index" :recent_courses_menu="element"
                            class="col-auto">
                            {{ element }}
                        </li>
                    </ul>
                    <ul class="row row-cols-6 list-unstyled">
                        <main_card v-for="element, index in getRecentsCourses" :key="index" :courses="element" />
                    </ul>
                </div>
                <div class="right-menu col-auto flex-column text-center">
                    <ul class="list-unstyled">
                        <main_side_menu v-for="element, index in side_menu_icons" :key="index" :side_menu_icons="element">
                        </main_side_menu>
                    </ul>
                </div>
            </div>
        </div>
</template>
<script>

import main_card from '../components/main_card.vue'
import main_side_menu from './main_side_menu.vue';
export default {
    name: 'main_recent_courses',
    props: ['recent_courses_menu', 'courses', 'side_menu_icons'],
    data() {
        return {
            click_more: true,
        }
    },
    components: {
    main_card,
    main_side_menu
},
    computed: {
        getRecentsCourses() {
            const recent_courses = this.courses.slice(0, 12);
            return recent_courses;
        }
    }
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';

// .btn {
//     color: $coral-red;
// }

.right-menu {
    position: absolute;
    top: 78%;
    right: 13px;
    box-shadow: 4px 0px 22px 5px #888888;
}
</style>