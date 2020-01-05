<template>
    <div class="content" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
         data-sal-easing="ease-out-bounce">
        <div class="Section">
            <h2 class="Section__title" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                data-sal-easing="ease-out-bounce">{{ title }}</h2>
            <div class="Section__content">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script>
    import sal from 'sal.js';

    export default {
        props: ['title'],
        mounted() {
            this.$nextTick(() => sal());
        }
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');

    .Section {
        position: relative;

    }

    .Section__title {
        width: 100%;
        padding-top: 0.25rem;
        font-size: 5rem;
        font-family: 'Montserrat', sans-serif;
        font-weight: 700;
        color: RGBA(49, 79, 64, 0.15);

    }

    .Section__content {
        width: 100%;
        max-width: 38rem;
        margin-top: 3.665rem;

    }

    .content {
        margin-top: -3.5rem;
    }

    @media (max-width: 667px) {

        .Section {
            display: contents;
        }

        .Section__title {
            width: 100%;
            font-size: 3.5rem;
            margin-top: 4rem;

        }

        .Section__content {
            width: 100%;
            margin-top: 2rem;
        }
    }

</style>
