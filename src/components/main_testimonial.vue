<template>
    <div class="testimonial container-fluid position-relative mt-5">
        <div class="row h-100 align-items-center justify-content-center">
            <div class="text-banner col-5">
                <h3>Investing for Your Future</h3>
                <p class=" mt-4 mb-4">It is no exageration to say this Masterstudy
                    experience was trasformative-both professionally and personally. This
                    workshop will long remain a high point of my life. Thanks again... I am
                    feeling energized and eager to start teaching my class next week. I
                    can't wait to use all of my new teaching tools. I will absolutely
                    recommend this workshop to other educators!</p>
                <div class="fw-bold">Linda Green</div>
                <div class="signed">Product Manager, Apple Inc</div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'main_testimonial',
}
</script>
<style lang="scss" scoped>
.testimonial {
    background-image: url("./../assets/images/testimonial-1-1917x640-1-1914x639.jpg");
    background-size: cover;
    background-position: center;
    height: 70vh;

    .text-banner {
        background-color: white;
        position: absolute;
        top: 10%;
        left: 20%;
        padding: 50px;
        line-height: 1.5em;

        .signed {
            font-size: 0.8em;
            line-height: 0;
        }
    }
}
</style>