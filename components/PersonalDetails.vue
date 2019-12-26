<template>
    <div class="content">
        <div class="Section">
            <div>
                <img class="portrait" src="../assets/matthiaskoch.jpg">
            </div>

            <h2 class="Personal__title">{{ title }}</h2>
            <div class="Personal__subtitle">
                <h3>Name:</h3>
                <h3>Mail:</h3>
                <h3>Residence:</h3>
                <h3>Date of birth:</h3>
                <h3>Nationality:</h3>
                <h3>Hobbys:</h3>
            </div>

            <div class="Personal__content info">
                <p>Matthias Koch</p>
                <p><a href="mailto:hello@matthiasko.ch">hello@matthiasko.ch</a></p>
                <p>Zug, Switzerland</p>
                <p>23.04.1996</p>
                <p>Swiss</p>
                <p>⛷🧗🏽‍♂️🏋🏽🗺📷</p>
            </div>

        </div>
    </div>
</template>

<script>

    export default {
        props: ['title']
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');
    @import url('https://fonts.googleapis.com/css?family=Nunito:400,700&display=swap');


    .Section {
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

    .Personal__subtitle {
        font-family: 'Nunito', sans-serif;
        font-weight: 700;
        font-size: 1.125rem;
        line-height: 1.575rem;
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

    .Personal__subtitle h3{
        padding-bottom: 0.75rem;
    }

    .content {
        margin-top: -4rem;
    }

    .portrait{
        position: absolute;
        margin-top: 4.5rem;
        right: 2rem;
        width: 37%;
    }

    @media (max-width: 667px) {

        .Section {
            display: contents;
        }

        .Personal__title {
            width: 100%;
            margin-top: -37.25rem;
            position: absolute;
        }

        .Personal__subtitle{
            width: 100%;
            margin-top: 3rem;
            position: relative;
        }

        .Personal__content {
            width: 100%;
            margin-top: 3rem;
            position: relative;

        }

        .portrait{
            position: relative;
            margin-top: 10.6rem;
            width: 100%;
            right: 0;
        }
    }

</style>
