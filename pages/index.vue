<template>
    <div class="container">
        <section class="panel header">
            <headerSection/>
        </section>

        <section class="panel inhalt">
            <div class="content">
                <h2 class="lead">My name is Matthias Koch, I am 23 years old and currently studying interaction design
                    at
                    the
                    School for Design Zürich. Next to my study I work as an interaction designer to help building better
                    digital
                    products.</h2>
                <hr>


                <Section title="Experience">
                    <p class="what"><strong>Interaction Design & Photography </strong><br>@ internezzo ag (2017 - 2019)
                    </p>

                    <p class="what"><strong>Event Management Internship & Photography</strong>
                        <br>@ Küssenberger & Partner (2016 - 2017)</p>

                    <p class="what"><strong>Fotofachmann EFZ</strong>
                        <br>@ Foto Studio Kasino ag (2012 - 2015)</p>
                </Section>

                <hr>

                <Section title="Education">
                    <p class="what"><strong>HF Interaction Design</strong>
                        <br>@ Schule für Gestaltung Zürich (2017 - 2020)</p>

                    <p class="what"><strong>Cambridge First Certificate</strong>
                        <br>@ Selc Syndey, Australia (2015 - 2016)</p>

                    <p class="what"><strong>Fotofachmann EFZ</strong>
                        <br>@ Medien Form & Farbe (2012 - 2015)</p>
                </Section>

                <hr>

                <Section title="Skills">
                    <p><strong>Design:</strong><br> Sketch, Figma, Adobe XD, Protopie, Adobe Photoshop, Illustrator,
                        InDesign, Premiere Pro,
                        After Effects</p>
                    <p><strong>Code:</strong><br> Basic HTML, CSS and Javascript</p>
                    <p><strong>Tools I like:</strong><br> Jira, Confluence, Slack, Bear</p>
                </Section>

                <hr>

                <Section title="Languages">
                    <p>Swiss German: Native</p>
                    <p>German: Fluent</p>
                    <p>English: Fluent</p>
                </Section>

                <hr>

                <h2 class="contact">Matthias Koch // <a href="mailto:hello@matthiasko.ch">hello@matthiasko.ch</a></h2>
            </div>
        </section>
    </div>

</template>

<script>

    import headerSection from "../components/headerSection";

    import Section from "../components/Section";

    export default {
        components: {
            headerSection,
            Section
        }
    }

</script>

<style>
    @import url('https://fonts.googleapis.com/css?family=Nunito+Sans:300,400,700&display=swap');

    .lead {
        font-family: 'Nunito Sans', sans-serif;
        font-weight: 300;
        font-size: 1.625rem;
        margin: auto;
        padding-top: 100px;
    }

    .background {
        background-color: white;
        z-index: 1;
    }

    .content {
        max-width: 56.875rem;
        margin: 0 auto;
        padding: 15px;
    }

    hr {
        margin: auto;
        margin-top: 6.25rem;
        margin-bottom: 3.125rem;
        border: 1x solid #CCCCCC;
    }

    p {
        font-family: 'Nunito Sans', sans-serif;
        font-size: 1.125rem;
        line-height: 1.575rem;
        padding-bottom: 1.5rem;
    }

    h3 {
        font-family: 'Nunito Sans', sans-serif;
        font-size: 1.325rem;
    }

    h2 {
        font-family: 'Nunito Sans', sans-serif;
        font-size: 1.825rem;
    }

    .contact {
        font-family: 'Nunito Sans', sans-serif;
        font-weight: 300;
        font-size: 1.125rem;
        margin-bottom: 3.125rem;
    }

    html {
        overflow-x: hidden;
    }
</style>
