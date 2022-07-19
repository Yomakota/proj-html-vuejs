<template>
    <section id="news-letter">
        <div class="subscribe container-fluid">
            <div class="row align-items-center justify-content-center">
                <div class="col-8 py-5">
                    <div class="row row-cols-2 text-white">
                        <div class="col-6">
                            <h5>Subscribe our newsletter</h5>
                            <p class="fs-7">There are variations of passages of Lorem Ipsum available, but the majority
                                have
                                suffered alteration in some form, by injected humour, or randomised words</p>
                        </div>
                        <div class="col-6 text-uppercase">
                            <div class="mb-1">
                                your e-mail address
                            </div>
                            <input class="w-75 p-2" placeholder="Enter your E-mail" type="text">
                            <button class="p-2 border-0 text-uppercase">subscribe</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'main_newsLetter'
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';

.subscribe {
    background-color: $coral-red;
    font-size: 0.9em;

    .fs-7 {
        font-size: .7em;
    }

    button {
        background-color: $oxford-blue;
        color: white;
    }
}
</style>