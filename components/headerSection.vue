<template>
    <div class="headerSection">
        <h1 class="title"
            data-sal="slide-up"
            data-sal-delay="100"
            data-sal-duration="1000"
            data-sal-easing="ease-out-bounce">

            I simplify technology</h1>

        <h2 class="titlelead"
            data-sal="slide-up"
            data-sal-delay="100"
            data-sal-duration="1000"
            data-sal-easing="ease-out-bounce">

            Hi, my name is Matthias Koch, I am a 23 years old Interaction Designer, currently working
            <a href="https://www.swisscom.com" target="_blank">@ Swisscom</a><br> to help building better digital products.</h2>
    </div>
</template>

<script>
    import sal from 'sal.js';

    export default {
        mounted () {
            this.$nextTick(() => sal());
        }
    }

</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');

    .headerSection {
        width: 100vw;
        height: 100vh;
        background-color: #0E0E0E;
    }

    .title {
        max-width: 43rem;
        padding: 2rem;
        padding-top: 18rem;
        padding-bottom: 0rem;
        margin: auto;
        text-align: left;
        font-family: 'Montserrat', sans-serif;
        font-weight: 400;
        font-size: 3.5rem;
        background: -webkit-linear-gradient(45deg, #E859FF, #FFBA2E);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .titlelead{
        max-width: 43rem;
        margin: auto;
        padding: 2rem;
        text-align: left;
        font-weight: 300;
        font-family: 'Montserrat', sans-serif;
        color: #ffffff;
        font-size: 1.5rem;
    }

    a{
        background: -webkit-linear-gradient(45deg, #E859FF, #FFBA2E);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

</style>
