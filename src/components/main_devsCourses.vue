<template>
    <div class="container_fluid">
        <div class="row justify-content-center">
            <div class="col-11">
                <h3 class="my-5">
                    Popular Development Courses
                </h3>

                <ul class="row row-cols-6 g-4 list-unstyled">
                    <main_card v-for="element, index in getDevCourses" :key="index" :courses="element" />
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
import main_card from './main_card.vue'
export default {
    name: "main_devsCourses",
    props: ['courses'],
    components: {
        main_card,
    },
    data() {
        return {};
    },
    computed: {
        getDevCourses() {
            const devCourses = this.courses.filter((element) => {
                return element.category === "development";
            });
            return devCourses;
        }
    },
}
</script>
<style lang="scss">
</style>