<template>
    <div id="header-main" class="container-fluid">
        <div class="row justify-content-center">
            <div class="col-11 py-3">
                <div class="row row-cols-4 align-items-center justify-content-between">
                    <div class="col-2">
                        <img class="w-100" src="../assets/images/MasterStudy.svg" alt="MasterStudy">
                    </div>
                    <div class="col-5">
                        <div class="input-group align-items-center">
                            <button class="btn btn-outline">
                                <i class="fas fa-bars fs-10 me-1"></i>
                                <span class="text-uppercase fs-10 me-1">category</span>
                            </button>
                            <input type="text" class="form-control input-field p-2" placeholder="Search courses">
                            <button class="btn-search input-group-text btn btn-primary-outline px-3 py-2">
                                <i class="icon-search-color fas fa-search"></i>
                            </button>
                        </div>
                    </div>
                    <div class="col-3">
                        <div class="row row-cols-2 g-0">
                            <div class="col-6">
                                <a class="btn btn-outline">
                                    <i class="fas fa-bullhorn me-1"></i>
                                    <span class="fs-10">Became an instructor</span>
                                </a>
                            </div>
                            <div class="col-6">
                                <a class="btn btn-outline">
                                    <i class=" fas fa-briefcase me-1"></i>
                                    <span class="fs-10">For Enterprise</span>
                                </a>
                            </div>
                        </div>
                    </div>
                    <div class="col-2 user-action">
                        <div class="log-in row row-cols-3 align-items-center justify-content-between g-0">
                            <a class="col-auto">
                                <i class="far fa-user me-1"></i>
                                <span class="fs-10">Log In</span>
                            </a>
                            <a class="col-auto">
                                <button type="button"
                                    class="sign-up btn btn-outline-danger rounded-pill text-uppercase fw-bold p-3">
                                    <span class="fs-6">
                                        sign up
                                    </span>
                                </button>
                            </a>
                            <a class="col-auto">
                                <i class="fs-4 far fa-bookmark"></i>
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

#header-main {
    color: $venus;

    .fs-10 {
        font-size: 10px;
    }

    .btn.btn-outline{
        color: $venus;
    }
    .input-field {
        background-color: $mystic;
    }
    .btn-search {
        background-color: $oxford-blue;

        .icon-search-color {
            color: white;
        }
    }
    .sign-up:hover {
        background-color: $coral-red;
    }
}
</style>