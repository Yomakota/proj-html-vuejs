<template>
    <div id="header-main" class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-11 py-3">
                <div class="row row-cols-4 gx-1 align-items-center justify-content-between">
                    <div class="col-2">
                        <img src="../assets/images/MasterStudy.svg" alt="">
                    </div>
                    <div class="col-5">
                        <div class="input-group align-items-center">
                            <button class="color-button btn btn-outline">
                                <i class="me-1 fas fa-bars"></i>
                                <span class="me-3 text-uppercase fs-6">category</span>
                            </button>
                            <input type="text" class="color form-control p-3" placeholder="Search courses">
                            <button class="input-group-text btn btn-primary-outline px-4 py-3">
                                <i class="icon-color fas fa-search"></i>
                            </button>
                        </div>
                    </div>
                    <div class="col-3">
                        <a class="color-button btn btn-outline">
                            <i class="me-1 fas fa-bullhorn"></i>
                            <span class="me-3">Became an instructor</span>
                        </a>
                        <a class="color-button btn btn-outline">
                            <i class="me-1 fas fa-briefcase"></i>
                            <span>For Enterprise</span>
                        </a>
                    </div>
                    <div class="col-2">
                        <div class="row align-items-center justify-content-between">
                            <a class="col-4">
                                <i class="far fa-user"></i>
                                <span>Log In</span>
                            </a>
                            <a class="col-6">
                                <button type="button" class="sign-up rounded-pill px-4 py-3 text-uppercase">
                                    sign up
                                </button>
                            </a>
                            <a class="col-2">
                                <i class="fs-3 far fa-bookmark"></i>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'header_Main'
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';


.form-control::placeholder {
    color: $venus;
}
.color{
    background-color: $mistic;
}

.btn.btn-primary-outline{
    background-color: $azure;
    .icon-color{
        color: white;
        font-size: 25px;
    }
}

.color-button{
    color: $venus;
}

.sign-up{
    color: white;
    background-color: $coral-red;
}
</style>