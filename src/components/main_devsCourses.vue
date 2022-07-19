<template>
    <section id="development-courses">
        <div class="container_fluid mt-5">
            <div class="row justify-content-center">
                <div class="col-11">
                    <h3 class="fs-5 fw-bold mb-4">
                        Popular Development Courses
                    </h3>
                    <div>
                        <ul class="row row-cols-6 g-3 list-unstyled">
                            <main_card v-for="element, index in getDevCourses" :key="index" :courses="element" />
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import main_card from './main_card.vue'
export default {
    name: "main_devsCourses",
    props: ['courses'],
    components: {
        main_card,
    },
    computed: {
        getDevCourses() {
            const devCourses = this.courses.filter((element) => {
                return element.category === "Development >";
            });
            return devCourses;
        }
    },
}
</script>
<style lang="scss">
</style>