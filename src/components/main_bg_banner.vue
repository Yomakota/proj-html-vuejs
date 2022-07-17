<template>
    <div class="container-fluid bg-banner">
        <div class="row h-100 align-items-center">
            <div class="col-6">
                <div class="row justify-content-end">
                    <div class="col-7">
                        <h2 class="fs-7 pe-6">Limitless learning, more possibilities</h2>
                        <p class="fs-6">Online courses open the oppurtinity for learning to almost anyone,
                            regardless of
                            their scheduling commitments
                        </p>
                        <button type="button" class="btn-read-more rounded-pill text-light px-4 py-3">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
name: 'main_bg_banner',
}
</script>
<style lang="scss">
@import '../assets/scss/style.scss';
.bg-banner {
    background-image: url('../assets/images/bg.png');
    background-size: cover;
    background-position: center;
    height: 50vh;
    .fs-7{
        font-size: 3.5em;
    }

    .btn-read-more{
        background-color: $coral-red;
    }
}
</style>