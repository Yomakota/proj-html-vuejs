<template>
    <section id="pops-courses">
        <div id="popular-courses" class="container-fluid mb-5 py-5">
            <div class="row justify-content-center">
                <div class="col-11">
                    <div class="title mb-5 text-center">
                        <h2 class="fw-bold fs-1">Popular courses</h2>
                        <h3 class="fw-light fs-6">Discover our most popular courses for self learning</h3>
                    </div>
                    <div>
                        <ul class="row row-cols-6 list-unstyled">
                            <main_card v-for="element, index in getPopsCourses" :key="index" :courses="element" />
                        </ul>
                    </div>
                </div>
                <div class="row my-5">
                    <div class="col text-center">
                        <button class="px-3 py-2">
                            <i class="fas fa-angle-left"></i>
                        </button>
                        <button class="px-3 py-2">
                            <i class="fas fa-angle-right"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>
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
<style lang="scss" scoped>
@import'../assets/scss/style.scss';

#popular-courses {
    background-color: $mystic;

    button {
        background-color: $white;
        border-color: $mystic;
        color: $mystic;
        font-size: 1.5em;

        &:hover {
            background-color: $oxford-blue;
            color: $mystic;
        }
    }
}

</style>