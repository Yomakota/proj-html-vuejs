<template>
    <li class="col p-2 text-center">
        <a href="#">
            <i class="fs-6" :class="'fas' + ' ' + side_menu_icons"></i>
        </a>
    </li>
</template>
<script>


export default {
    name: 'main_side_menu',
    props: ['side_menu_icons']
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';
    li{
        &:hover{
            background-color: $mystic;
        }
    }
</style>