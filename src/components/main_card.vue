<template>
    <li class="col my-5">
        <div class="card">
            <div class="card-img-top">
                <img :src="courses.img" :alt="courses.description" class="w-100">
            </div>
            <div>
                <div class="card-body p-3">
                    <div class="category fs-7 pb-2">
                        {{ courses.category }}
                    </div>
                    <div class="description-card border-bottom">
                        {{ courses.description }}
                    </div>
                    <div class="row align-items-center">
                        <div class="col card-bottom">
                            <img v-for=" index in 5" :key="index" :src="(index <= courses.vote) ?
                            require('../assets/images/starfull.svg') :
                            require('./../assets/images/staremptyl.svg')" :alt="courses.vote">
                        </div>
                        <div class="full-price col text-end">
                            <div class="text-decoration-line-through">
                                {{ courses.full_price }}
                            </div>
                            <div class="discount">
                                {{ courses.discounted_price }}
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </li>
</template>
<script>
export default {
    name: 'main_card',
    props: ['courses'],
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
</style>