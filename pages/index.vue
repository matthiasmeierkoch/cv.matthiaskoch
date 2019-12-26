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
        margin-right: 2rem;
        margin-left: 2rem;
    }

    .sectionHeader {
        top: 0;
        z-index: -1;

    }

    html {
        overflow-x: hidden;
    }
</style>
