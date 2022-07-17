<template>
    <li class="col social_color">
        <a :class="footer_socials.color">
            <i :class="'fab ' + footer_socials.icon"></i>
        </a>
    </li>
</template>
<script>
export default {
    name: 'footer_SocialLinks',
    props:['footer_socials']
}
</script>
<style lang="scss" scoped>
@import '../assets/scss/style.scss';

.social_color a {
    padding: 6px 11px;
    border-radius: 30px;

    &.facebook {
        background-color: $azure;
    }

    &.instangram {
        background-color: $instangram;
    }

    &.linkedin {
        background-color: $boston-blue;
    }

    &.pinterest {
        background-color: $amaranth;
    }

    &.twitter {
        background-color: $twitter;
    }

    &.dribble {
        background-color: $dribble;
    }

    &.google {
        background-color: $coral-red;
    }

    &.skype {
        background-color: $half-baked;
    }
}
</style>