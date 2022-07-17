<template>
    <div class="container-fluid position-relative my-5">
        <div class="row justify-content-center">
            <div class="col-11 text-center">
                <h1>Popular courses</h1>
                <h2>Discover our most popular courses for self learning</h2>
                <ul class="row row-cols-6 list-unstyled">
                    <main_card v-for="element, index in getPopsCourses" :key="index" :courses="element" />
                </ul>
            </div>
            <div>
                <button>
                </button>
                <button>

                </button>
            </div>
        </div>
    </div>
</template>
<script>
import main_card from './main_card.vue';
export default {
    name: 'main_popsCourses',
    props: ['courses'],
    components: {
        main_card,
    },
    computed: {
        getPopsCourses() {
            const popular_courses = this.courses.slice(0, 6);
            return popular_courses;
        }
    }
}
</script>
<style lang="scss">

</style>