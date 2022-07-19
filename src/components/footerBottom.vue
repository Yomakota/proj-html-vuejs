<template>
    <div id="footer-bottom" class="container-fluid border-top">
        <div class="row justify-content-center text-white">
            <div class="col-8 pt-4">
                <div class="row row-cols-2">
                    <div class=" col-auto footer-logo">
                        <img class="w-100 me-3" src="./../assets/images/footer-logo2x-50x56.png" alt="master-study">
                    </div>
                    <div class="col-auto copyright">
                        <span>Copyright &#169; 2020</span>
                        <a class="text-white ms-2 me-2 text-decoration-underline" href="#">Masterstudy</a>
                        <span>Theme by</span>
                        <a class="text-white ms-2 text-decoration-underline" href="#">StyleMixThemes</a>
                    </div>
                </div>
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
.footer-logo{
    width: 50px;
    height: 50px;
}
</style>