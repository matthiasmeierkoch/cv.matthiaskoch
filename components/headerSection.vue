<template>
    <div class="headerSection">
        <div class="nav">
            <h2 class="name">Matthias Koch</h2>
            <h2 class="path"> / Crriculum Vitae</h2>
        </div>

        <h1 class="title">Curriculum Vitae</h1>
        <div class="section">
            <span class="hscroll-line"></span>
        </div>
    </div>
</template>

<script>

    export default {}

</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Montserrat&display=swap');

    .headerSection {
        width: 100vw;
        height: 100vh;
        background-color: #0E0E0E;
        }

    .nav {
        display: flex;
    }

    .name {
        padding-top: 4rem;
        padding-left: 2rem;
        color: #ffffff;
        font-family: 'Montserrat', sans-serif;
        font-size: 1.25rem;
        font-weight: 300;
    }

    .path {
        padding-top: 4rem;
        margin-left: 0.5rem;
        color: #ffffff;
        font-family: 'Montserrat', sans-serif;
        font-size: 1.25rem;
        font-weight: 700;
    }

    @media (max-width: 667px) {
        .name {
            font-size: 0.9rem;
        }

        .path {
            font-size: 0.9rem
        }

        .title{
            font-size: 2rem;
            padding-top: 40%;
        }

        .hscroll-line{
            bottom: 40%;
        }
    }

    .title {
        width: 100%;
        padding-top: 35vh;
        margin: auto;
        text-align: center;
        font-family: 'Montserrat', sans-serif;
        font-size: 3.5rem;
        background: -webkit-linear-gradient(45deg, #E859FF, #FFBA2E);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .section {
        width: 80%;
        margin: 0 auto;
        height: 50%;
        position: relative;
        padding: 0
    }

    .hscroll-line {
        bottom: 20%;
        right: 50%;
        height: 2px;
        position: absolute;
        overflow: hidden;
        width: 60px;
        transform: rotate(90deg);
        tranform-origin: 50% 50%;

    }

    .hscroll-line::before,
    .hscroll-line::after {
        position: absolute;
        top: -50px;
        left: 0;
        right: 0;
        bottom: 0;
        content: ""
    }

    .hscroll-line:before {
        background: #ffffff3b;
    }

    .hscroll-line::after {
        background: #FFBA2E;
        animation: move 3s infinite
    }

    @keyframes move {
        0% {
            transform: translate3d(-200%, 0, 0)
        }
        60% {
            transform: translate3d(100%, 0, 0)
        }
        100% {
            transform: translate3d(100%, 0, 0)
        }
    }

</style>
