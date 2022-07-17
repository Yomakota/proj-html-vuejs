<template>
    <div id="header-top" class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-11 py-3">
                <div class="row align-items-center">
                    <div id="language" class="col-2">
                        <span class="m-2">English</span>
                        <i class="fas fa-angle-down"></i>
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
    border-bottom: 1px solid $venus;
}
</style>