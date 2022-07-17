<template>
    <div>
        <div class="jumbotron my-4 container-fluid">
            <div class="row h-100">
                <div class="col-12 text-light cover-jumbo position-relative">
                    <!-- img jumbo -->
                    <img class="h-100 w-50" src="../assets/images/slide-1.jpg" alt="Affiliate Sales">
                    <div class="row h-100 align-items-center justify-content-center">
                        <div class="col-8">
                            <div class="row">
                                <div class="col-6">
                                    <h2 class="fw-bolder fs-1 mb-4">Udemy Affiliate Sales</h2>
                                    <h3 class="fs-5">Monetize your audience and attract new customers with Udemy!</h3>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'main_JumboTron'
}
</script>

<style lang="scss">
@import '../assets/scss/style.scss';
.jumbotron {
    height: 400px;

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