<template>
    <li class="col p-3 text-center">
        <a href="#">
            <i class="fs-3" :class="'fas' + ' ' + side_menu_icons"></i>
        </a>
    </li>
</template>
<script>


export default {
    name: 'main_side_menu',
    props: ['side_menu_icons']
}
</script>
<style lang="scss">

</style>