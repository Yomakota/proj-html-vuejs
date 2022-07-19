<template>
    <li class="col mb-3">
        <div class="card h-100">
            <div class="card-img-top">
                <img :src="courses.img" :alt="courses.description" class="w-100">
            </div>
            <div>
                <div class="card-body p-2">
                    <div class="category text-black-50 fs-small pb-2">
                        {{ courses.category }}
                    </div>
                    <div class="description border-bottom fs-7 pb-2">
                        {{ courses.description }}
                    </div>
                    <div class="row align-items-center">
                        <div class="col card-bottom">
                            <img v-for=" index in 5" :key="index" :src="(index <= courses.vote) ?
                            require('../assets/images/starfull.svg') :
                            require('./../assets/images/staremptyl.svg')" :alt="courses.vote">
                        </div>
                        <div class="full-price col text-end">
                            <div class="text-decoration-line-through text-black-50 fs-small">
                                {{ courses.full_price }}
                            </div>
                            <div class="discount fs-7">
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

.fs-7{
    font-size: .7em;
}

.fs-small{
    font-size: .5em;
}
</style>