<template>
    <li class="fs-6">
        <a class="mx-2" href="#">
            <i :class="'fab'+' '+ social_links"></i>
        </a>
    </li>
</template>
<script>
export default {
    name: 'header_SocialIcons',
    props: ['social_links']
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

li{
    a{
        color: #AAAAAA;
    }
}
</style>