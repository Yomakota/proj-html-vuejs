<template>
    <div class="container-fluid footer-top py-3 text-light">
        <div class="row justify-content-center">
            <div class="col-8">
                <div class="row row-cols-4">
                    <div class="col">
                        <h5>ABOUT</h5>
                        <p class="fs-08">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo asperiores ad
                            rerum? Commodi dignissimos vero qui molestiae velit alias assumenda quisquam molestias
                            lorem.</p>
                    </div>
                    <div class="col">
                        <h5>CONTACT</h5>
                        <div class="fs-08">
                            <div class="mb-3">USA, California 20, First Avenue, California</div>
                            <div>Tel: +1 212 458 300 32</div>
                            <div class="mb-3">Fax: +1 212 375 24 14</div>
                            <div class="e-mail">info@masterstudy.com</div>
                        </div>
                    </div>
                    <div class="col">
                        <h5>SOCIAL NETWORK</h5>
                        <ul class="list-unstyled row gy-3 row-cols-4">
                            <footer_socialsLinks v-for="element, index in footer_socials" :key="index"
                                :footer_socials="element" />
                        </ul>
                    </div>
                    <div class="col-3">
                        <div>
                            <img class="w-100" src="../assets/images/Top-udemy-courses-90-percent-off.jpg" alt="udemy-discount">
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
.footer-top{
    background-color: $oxford-blue;
}

.img_container{
    width: 20px;
    height: 20px;
}
// .contacts {
//     background-color: $oxford-blue;

//     .fs-08 {
//         font-size: 0.8em;
//     }

//     .e-mail {
//         color: $venus;
//     }

</style>