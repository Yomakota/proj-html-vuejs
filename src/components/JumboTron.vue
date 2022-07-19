<template>
    <section id="jumbotron" class="my-4">
        <div class="container-fluid">
            <div class="row">
                <div class="col-12 text-light cover-jumbo position-relative">
                    <div>
                        <img class="h-100 w-50" src="../assets/images/slide-1.jpg" alt="Affiliate Sales">
                    </div>
                    <div class="row align-items-center justify-content-center">
                        <div class="col-8 py-6">
                            <div class="row">
                                <div class="col-6">
                                    <h3 class="fw-bolder fs-1 mb-4">Udemy Affiliate Sales</h3>
                                    <h4 class="fs-6">Monetize your audience and attract new customers with Udemy!</h4>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'main_JumboTron'
}
</script>

<style lang="scss">
@import '../assets/scss/style.scss';
#jumbotron {
    .py-6{
        padding: 6em 0;
    }
    .cover-jumbo {
        background-image: linear-gradient(68deg, $coral-red 54%, transparent 1px);

        img {
            position: absolute;
            top: 0;
            right: 0;
            z-index: -1;
        }
    }
}
</style>