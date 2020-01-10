<template>
    <div class="container">

            <div class="sectionHeader">
                <headerSection/>
            </div>

            <div class="contentSection">
                <contentSection/>
            </div>

    </div>

</template>

<script>

    import Parallax from "vue-parallaxy";
    import headerSection from "../components/headerSection";
    import contentSection from "../components/contentSection";

    export default {
        components: {
            headerSection,
            Parallax,
            contentSection
        }
    }

</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Nunito+Sans:300,400,700&display=swap');


    .contentSection {
        z-index: 1;
        padding-right: 2rem;
        padding-left: 2rem;
        padding-bottom: 2rem;
        margin: 90vh 5vw 0vw 5vw;
        border-radius: 1.25rem 1.25rem 0 0 ;
        background-color: white;
    }

    .sectionHeader {
        top: 0;
        position: fixed;
        z-index: -1;

    }

    html {
            overflow-x: hidden;
        background-color: white;
    }
</style>
