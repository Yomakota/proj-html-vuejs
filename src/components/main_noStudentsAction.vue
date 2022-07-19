<template>
    <section id="actions-users">
        <div class="container-fluid">
            <div class="row justify-content-center">
                <div class="col-11">
                    <div class="row row-cols-2">
                        <div class="col-6">
                            <div class="card p-5">
                                <div class="row align-items-center justify-content-center">
                                    <div class="col-6">
                                        <img src="./../assets/images/image_box_1-221x231.png" alt="">
                                    </div>
                                    <div class="col-6">
                                        <div class="p-1">
                                            <h4>Become an Instructor</h4>
                                        </div>
                                        <div class="p-1">
                                            <p class="fs-7">Teach what you love. Masterstudy gives you the tools to
                                                create a
                                                course</p>
                                        </div>
                                        <div class="p-1">
                                            <button type="button"
                                                class="btn btn-danger rounded-pill text-uppercase shadow-none fw-bold fs-8 p-3">start
                                                teaching
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="col-6">
                            <div class="card p-5">
                                <div class="row align-items-center justify-content-center">
                                    <div class="col-6">
                                        <img src="./../assets/images/image_box_2-234x231.png" alt="">
                                    </div>
                                    <div class="col-6">
                                        <div class="p-1">
                                            <h4>Access For Business</h4>
                                        </div>
                                        <div class="p-1">
                                            <p class="mb-3 fs-7">Get unlimited access to 2,500 of top courses for your
                                                team
                                            </p>
                                        </div>
                                        <div class="p-1">
                                            <button type="button"
                                                class="btn btn-danger rounded-pill text-uppercase shadow-none fw-bold fs-8 p-3">doing
                                                business</button>
                                        </div>
                                    </div>
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
    name: 'main_noStudentsAction'
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';
.fs-7{
    font-size: .7em;
    color: $venus;
}

.fs-8{
    font-size: .8em;
}

.btn.btn-danger {
    background-color: $coral-red;
    &:hover{
        background-color: $forest-green;
    }
}
</style>