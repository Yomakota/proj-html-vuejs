<template>
    <div id="header-bottom-nav-menu" class="container-fluid">
        <div class="row justify-content-center py-4">
            <div class="col-11">
                <ul class="nav justify-content-center">
                    <header_BottomLinks v-for="element, index in nav_menu_links" :key="index"
                        :nav_menu_links="element" />
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
import header_BottomLinks from './header_BottomLinks.vue';

export default {
    name: 'header_BottomNavMenu',
    props: ['nav_menu_links'],
    components: {
        header_BottomLinks,
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#header-bottom-nav-menu{
    background-color: $ebony-clay;
    color: white;
}
</style>