<template>
    <div class="container-fluid border-top footer-bottom">
        <div class="row copyrigth text-white pt-3 pb-3 justify-content-center">
            <div class="col-8">
                <img class="me-3" src="./../assets/images/footer-logo2x-50x56.png" alt="master-study">
                <span>Copyrigth &#169; 2020</span>
                <a class="text-white ms-2 me-2" href="#">Masterstudy</a>
                <span>Theme by</span>
                <a class="text-white ms-2" href="#">StyleMixThemes</a>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'footer_bottom'
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';
.footer-bottom{
    background-color: $oxford-blue;
}
</style>