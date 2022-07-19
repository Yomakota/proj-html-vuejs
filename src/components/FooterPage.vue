<template>
    <footer>
        <footerTop :footer_socials="footer_socials" />
        <footerBottom/>
    </footer>
</template>
<script>

import footerTop from './footerTop.vue'
import footerBottom from './footerBottom.vue'
export default {
    name: 'FooterPage',
    components: {
        footerTop,
        footerBottom
    },
    props:['footer_socials']
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';
footer{
    background-color: $ebony-clay;
}
</style>