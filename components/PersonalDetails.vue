<template>
    <div class="content">
        <div class="Section_Personal">
            <h2 class="Personal__title" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                data-sal-easing="ease-out">
                {{ title }}</h2>
            <div>
                <img class="portrait" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                     data-sal-easing="ease-out"
                     src="../assets/matthiaskoch.jpg">
            </div>
                <div class="Personal__subtitle" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                     data-sal-easing="ease-out">
                    <h3>Name:</h3>
                    <h3>Mail:</h3>
                    <h3>Residence:</h3>
                    <h3>Date of birth:</h3>
                    <h3>Nationality:</h3>
                    <h3>Hobbys:</h3>
                </div>

                <div class="Personal__content info" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000"
                     data-sal-easing="ease-out" >
                    <p>Matthias Koch</p>
                    <p><a href="mailto:hello@matthiasko.ch">hello@matthiasko.ch</a></p>
                    <p>Zug, Switzerland</p>
                    <p>23.04.1996</p>
                    <p>Swiss</p>
                    <p>⛷ 🧗🏽‍♂ ️🏋🏽 🗺 📷</p>
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
    @import url('https://fonts.googleapis.com/css?family=Nunito:400,700&display=swap');

    .Section_Personal {
        position: relative;
        justify-content: space-between;
        display: flex;
    }

    .Personal__title {
        width: 100%;
        padding-top: 0.25rem;
        font-size: 4.5rem;
        font-family: 'Montserrat', sans-serif;
        font-weight: 700;
        position: absolute;
        color: RGBA(49, 79, 64, 0.15);

    }

    .Personal__subtitle h3 {
        font-family: 'Nunito', sans-serif;
        font-weight: 700;
        font-size: 1.125rem;
        line-height: 1.575rem;
    }

    .Personal__subtitle {
        width: 40%;
        margin-top: 7.5rem;
    }

    .Personal__content {
        font-family: 'Nunito', sans-serif;
        font-size: 1.125rem;
        line-height: 1.575rem;
        padding-bottom: 1.5rem;
        font-weight: 400;
        width: 120%;
        margin-top: 7.5rem;

    }

    .info p {
        padding-bottom: 0.76rem;
    }

    .Personal__subtitle h3 {
        padding-bottom: 0.75rem;
    }

    .content {
        margin-top: -4rem;
    }

    .portrait {
        position: absolute;
        margin-top: 4.5rem;
        right: 0%;
        max-width: 18rem;
    }

    @media (max-width: 667px) {

        .Personal__title {
            width: 100%;
            margin-top: 1rem;
            font-size: 3.5rem;
            position: absolute;
            line-height: 4rem;
        }

        .Personal__subtitle h3 {

        }

        .Personal__subtitle {
            width: 50%;
            margin-top: 30rem;
        }

        .Personal__content {
            width: 50%;
            margin-top: 30rem;
        }

        .portrait {
            position: absolute;
            right: 50%;
            margin-top: 10rem;
            width: 100%;
            left: 0%;

        }
    }

</style>
