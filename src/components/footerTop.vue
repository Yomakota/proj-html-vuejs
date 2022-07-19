<template>
    <div id="footer-top" class="container-fluid footer-top py-3 text-light">
        <div class="row justify-content-center">
            <div class="col-8">
                <div class="row row-cols-4 gx-5">
                    <div class="col">
                        <h5 class="text-uppercase">about</h5>
                        <p class="fs-8">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo asperiores ad
                            rerum? Commodi dignissimos vero qui molestiae velit alias assumenda quisquam molestias
                            lorem.</p>
                    </div>
                    <div class="col">
                        <h5 class="text-uppercase">contact</h5>
                        <div class="fs-8">
                            <div class="mb-3">USA, California 20, First Avenue, California</div>
                            <div>Tel: +1 212 458 300 32</div>
                            <div class="mb-2">Fax: +1 212 375 24 14</div>
                            <div class="e-mail">
                                <a href="#">
                                    info@masterstudy.com
                                </a>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <h5 class="text-uppercase mb-4">social network</h5>
                        <div>
                            <ul class="list-unstyled row gy-3 row-cols-4">
                                <footer_socialsLinks v-for="element, index in footer_socials" :key="index"
                                    :footer_socials="element" />
                            </ul>
                        </div>
                    </div>
                    <div class="col-3">
                        <div>
                            <img class="w-100" src="../assets/images/Top-udemy-courses-90-percent-off.jpg"
                                alt="udemy-discount">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import footer_socialsLinks from './footer_SocialLinks.vue'

export default {
    name: 'footerTop',
    props: ['footer_socials'],
    components: {
        footer_socialsLinks
    }
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';


.img_container {
    width: 20px;
    height: 20px;
}

.fs-8 {
    font-size: .8em;
}

.e-mail{
    color: $venus;
}
</style>