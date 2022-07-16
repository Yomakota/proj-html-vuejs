<template>
    <div id="header-nav-menu" class="container-fluid">
        <div class="row justify-content-center py-4">
            <div class="col-11">
                <ul class="nav justify-content-center">
                    <menuNavHeader v-for="element, index in nav_menu_links" :key="index" :nav_menu_links="element" />
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
import menuNavHeader from './menuNavHeader.vue';

export default {
    name: 'HeaderNavMenu',
    props: ['nav_menu_links'],
    components: {
        menuNavHeader,
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

#header-nav-menu{
    background-color: $ebony-clay;
    color: white;
}
</style>