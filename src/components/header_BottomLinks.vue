<template>
    <li class="fs-6">
        <a class="col mx-4" href="#">
            <i :class="'fas'+' '+ nav_menu_links.icon" class="mx-2"></i>
            <span>{{ nav_menu_links.text }}</span>
        </a>
    </li>
</template>
<script>
export default {
    name: 'header_BottomLinks',
    props: ['nav_menu_links']
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';

li{
    a:hover{
        color: $venus;
    }
}
</style>