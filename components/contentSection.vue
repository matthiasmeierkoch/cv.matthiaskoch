<template>

    <div class="sectionContent">
        <h2 class="lead" data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out">
            Thank you for showing interest in my CV, if you have any Questions, inquiries or would like
            to meet up for a Coffee please do not hesitate to Contact me.
            Cheers, Matthias!</h2>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">

        <PersonalDetails title="personal details">
        </PersonalDetails>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">


        <Section title="experience">
            <p class="what"><strong>Interaction Designer</strong><br>@ Swisscom ag (2019 - now)
            </p>

            <p class="what"><strong>Interaction Designer & Photography </strong><br>@ internezzo ag (2017 - 2019)
            </p>

            <p class="what"><strong>Event Management Internship & Photography</strong>
                <br>@ Küssenberger & Partner (2016 - 2017)</p>

            <p class="what"><strong>Fotofachmann EFZ</strong>
                <br>@ Foto Studio Kasino ag (2012 - 2015)</p>
        </Section>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">


        <Section title="education">
            <p class="what"><strong>HF Interaction Design</strong>
                <br>@ Schule für Gestaltung Zürich (2017 - 2020)</p>

            <p class="what"><strong>Cambridge First Certificate</strong>
                <br>@ Selc Syndey, Australia (2015 - 2016)</p>

            <p class="what"><strong>Fotofachmann EFZ</strong>
                <br>@ Medien Form & Farbe (2012 - 2015)</p>
        </Section>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">

        <Section title="competences">
            <p><strong>Design:</strong><br> Sketch, Figma, Adobe XD, Protopie, Adobe Photoshop, Illustrator,
                InDesign, Premiere Pro, After Effects</p>
            <p><strong>Code:</strong><br> Basic HTML, CSS and Javascript</p>
            <p><strong>Tools I like:</strong><br> Jira, Confluence, Slack, Bear</p>
        </Section>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">

        <Section title="languages">
            <p>Swiss German: Native</p>
            <p>German: Fluent</p>
            <p>English: Fluent</p>
        </Section>

        <hr data-sal="slide-up" data-sal-delay="100" data-sal-duration="1000" data-sal-easing="ease-out-bounce">

        <Section title="Contact">
            <p><a href="https://www.instagram.com/matthiasmeierkoch/">Instagram</a></p>
            <p><a href="https://www.linkedin.com/in/matthias-koch-3588ba119/">LinkedIn</a></p>
            <p><a href="mailto:hello@matthiasko.ch">E-mail</a></p>
        </Section>

        <weekday></weekday>
    </div>


</template>


<script>

    import Section from "../components/Section";
    import weekday from "../components/weekday";
    import sal from 'sal.js';
    import PersonalDetails from "../components/PersonalDetails";

    export default {
        components: {
            Section,
            PersonalDetails,
            weekday
        },

        mounted() {
            this.$nextTick(() => sal());
        }
    }

</script>


<style lang="scss">
    @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap');

    .lead {
        font-family: 'Nunito', sans-serif;
        font-weight: 300;
        font-size: 1.625rem;
        margin: auto;
        padding-top: 11.25rem;
    }

    .sectionContent {
        max-width: 46.875rem;
        margin: 0 auto;
        background: white;

    }

    hr {
        margin: auto;
        margin-top: 6.25rem;
        margin-bottom: 3.125rem;
        border: 1px solid RGBA(49, 79, 64, 0.15);
    }

    p {
        font-family: 'Nunito', sans-serif;
        font-size: 1.125rem;
        line-height: 1.575rem;
        padding-bottom: 1.5rem;
    }

    h3 {
        font-family: 'Nunito', sans-serif;
        font-size: 1.325rem;
    }

    h2 {
        font-family: 'Nunito', sans-serif;
        font-size: 1.825rem;
    }

    .contact {
        font-family: 'Nunito', sans-serif;
        font-weight: 300;
        font-size: 1.125rem;
        margin-bottom: 3.125rem;
    }

    html {
        overflow-x: hidden;
    }

    @media (max-width: 667px) {

        .lead {
            font-family: 'Nunito', sans-serif;
            font-weight: 300;
            font-size: 1.625rem;
            margin: auto;
            padding-top: 6rem;
        }
    }

</style>
