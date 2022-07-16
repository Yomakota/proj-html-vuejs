<template>
    <header class="header">
        <HeaderTopNav :links="links" :social_links="social_links" />
        <HeaderMain />
        <HeaderNavMenu :nav_menu_links="nav_menu_links" />
    </header>
</template>
<script>

import HeaderTopNav from './HeaderTopNav.vue'
import HeaderMain from './HeaderMain.vue'
import HeaderNavMenu from './HeaderNavMenu.vue'

export default {
    name: 'HeaderPage',
    components: {
        HeaderTopNav,
        HeaderMain,
        HeaderNavMenu,
    },
    props: ['links', 'social_links', 'nav_menu_links']
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
.header{
    background-color: $white;
    color: $venus;
}
</style>