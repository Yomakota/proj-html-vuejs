<template>
    <section id="bg-banner-learning">
        <div class="container-fluid bg-banner">
            <div class="row h-100 align-items-center">
                <div class="col-6">
                    <div class="row justify-content-end">
                        <div class="col-7 py-bg-banner">
                            <h2 class="fs-7 fw-bold">Limitless learning, more possibilities</h2>
                            <p class="fs-small">Online courses open the oppurtinity for learning to almost anyone,
                                regardless of
                                their scheduling commitments
                            </p>
                            <button type="button"
                                class="read-more btn btn-outline-danger rounded-pill text-uppercase fw-bold">
                                read more
                                </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
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
    .py-bg-banner{
        padding: 5.5em 0;
    }
    .fs-7{
        font-size: 2.5em;
    }
    .fs-small{
        font-size: .8em;
    }

    .read-more:hover{
        background-color: $coral-red;
    }

}
</style>