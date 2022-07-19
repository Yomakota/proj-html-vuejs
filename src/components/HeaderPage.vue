<template>
    <header class="header">
        <header_TopNavMenu :links="links" :social_links="social_links" />
        <header_Main />
        <header_BottomNavMenu :nav_menu_links="nav_menu_links" />
    </header>
</template>
<script>

import header_TopNavMenu from './header_TopNavMenu.vue'
import header_Main from './header_Main.vue'
import header_BottomNavMenu from './header_BottomNavMenu.vue'

export default {
    name: 'HeaderPage',
    components: {
        header_TopNavMenu,
        header_Main,
        header_BottomNavMenu,
    },
    props: ['links', 'social_links', 'nav_menu_links']
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
</style>