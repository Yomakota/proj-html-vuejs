<template>
    <section id="testimonial-banner">
        <div class="testimonial container-fluid mt-5 d-flex align-items-center justify-content-center py-4">
            <div class="row justify-content-center">
                <div class="col-8">
                    <div class="row p-5">
                        <div class="col-8 text-banner">
                            <h3>Investing for Your Future</h3>
                            <p class="text-p mt-4 mb-4">It is no exageration to say this MasterStudy
                                experience was trasformative-both professionally and personally. This
                                workshop will long remain a high point of my life. Thanks again... I am
                                feeling energized and eager to start teaching my class next week. I
                                can't wait to use all of my new teaching tools. I will absolutely
                                recommend this workshop to other educators!
                            </p>
                            <div class="fw-bold pb-1">Linda Green</div>
                            <div class="signed">Product Manager, Apple Inc.</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: 'main_testimonial_banner',
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

.testimonial {
    background-image: url("./../assets/images/testimonial-1-1917x640-1-1914x639.jpg");
    background-size: cover;
    background-position: center;

    .text-banner {
        background-color: white;
        padding: 40px;
        line-height: 1.5em;

        .text-p {
            color: $venus;
        }

        .signed {
            font-size: 0.8em;
            line-height: 0;
        }
    }
}
</style>