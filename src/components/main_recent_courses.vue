<template>
    <section id="recents-courses">
        <div class="container-fluid position-relative my-5">
            <div class="row justify-content-center">
                <div class="col-11">
                    <h2 class="text-center fw-bold fs-1">Recent courses</h2>
                    <div>
                        <ul class="recents-courses-links row row-cols-8 justify-content-center list-unstyled g-0 my-4">
                            <li v-for="element, index in recent_courses_menu" :key="index"
                                :recent_courses_menu="element" class="col-auto rounded-pill px-3 py-2 mb-3">
                                <a href="#">
                                    {{ element }}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul class="row row-cols-6 list-unstyled g-3">
                            <main_card v-for="element, index in getRecentsCourses" :key="index" :courses="element" />
                        </ul>
                        <ul v-if="click_more" class="row row-cols-6 list-unstyled g-3">
                            <main_card v-for="element, index in getRestCourses" :key="index" :courses="element" />
                        </ul>
                    </div>
                    <div class="row">
                        <div class="col-12 text-center">
                            <button @click="click_more = !click_more" type="button"
                                class="btn btn-outline-danger rounded-pill text-uppercase">{{ click_more == false ?
                                "show all"
                                :
                                "reduce"}}</button>
                        </div>
                    </div>
                </div>
                <div class="right-menu col-auto flex-column text-center shadow p-2 mb-5 bg-body rounded">
                    <ul class="list-unstyled">
                        <main_side_menu v-for="element, index in side_menu_icons" :key="index"
                            :side_menu_icons="element">
                        </main_side_menu>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>
<script>

import main_card from '../components/main_card.vue'
import main_side_menu from './main_side_menu.vue';
export default {
    name: 'main_recent_courses',
    props: ['recent_courses_menu', 'courses', 'side_menu_icons'],
    data() {
        return {
            click_more: false,
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
        },
        getRestCourses() {
            const all_courses = this.courses.slice(12, this.courses.length);
            return all_courses;
        }
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

.recents-courses-links{
    color: $venus;
    li{
        &:hover,
        &.clicked{
            background-color: $mistic;
        }
    }
}

.right-menu {
    position: absolute;
    top: 70%;
    right: 1%;
}
</style>