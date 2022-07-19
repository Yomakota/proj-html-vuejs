<template>
    <div id="header-top" class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-11 py-1">
                <div class="row align-items-center">
                    <div class="col-2">
                        <label class="align-middle m-2">English</label>
                        <button class="btn btn-outline p-0">
                            <i class="fas fa-angle-down"></i>
                        </button>
                    </div>
                    <div id="nav-menu" class="nav col-10 align-items-center justify-content-end">
                        <div>
                            <ul class="nav">
                                <li class="me-3" v-for="element, index in links" :key="index" :text="element">
                                    <a href="#">
                                        {{ element }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <ul class="nav ms-2">
                                <header_SocialIcons v-for=" element, index in social_links" :key="index"
                                    :social_links="element" />
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
import '@fortawesome/fontawesome-free/js/all.js';
import header_SocialIcons from './header_SocialIcons.vue';

export default {
    name: "header_TopNavMenu",
    components: {
        header_SocialIcons,
    },
    props: ['links', 'social_links']
}
</script>

<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#header-top{
    color: $mystic;
    font-size: 12px;
    border-bottom: 1px solid $mystic;
}
.btn.btn-outline {
    color: $mystic;
}
</style>