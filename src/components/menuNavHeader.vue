<template>
    <li class="fs-5">
        <a class="col mx-4" href="#">
            <i :class="'fas'+' '+ nav_menu_links.icon" class="mx-2"></i>
            <span>{{ nav_menu_links.text }}</span>
        </a>
    </li>
</template>
<script>
export default {
    name: 'menuNavHeader',
    props: ['nav_menu_links']
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
</style>