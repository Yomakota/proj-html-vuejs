<template>
    <div class="subscribe container-fluid">
        <div class="row h-100 align-items-center justify-content-center">
            <div class="col-8 p-5">
                <div class="row row-cols-2 text-white">
                    <div class="col-7">
                        <h4>Subscribe our newsletter</h4>
                        <p>There are variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words</p>
                    </div>
                    <div class="col-5 text-uppercase">
                        <div class="mb-3">
                            your email address
                        </div>
                        <input class="w-75 p-2" placeholder="Enter your E-mail" type="text">
                        <button class="p-2 text-uppercase">subscribe</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name:'main_newsLetter'
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
        .subscribe {
            background-color: $coral-red;
            font-size: 0.9em;

            button {
                background-color: $azure;
                color: white;
            }
        }
</style>