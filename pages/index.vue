<template>
  <div class="container">
    <headerSection/>

    <div class="content">
      <h2 class="lead">My name is Matthias Koch, I am 23 years old and currently studying interaction design at the
        School for Design Zürich. Next to my study I work as an interaction designer to help building better digital
        products.</h2>
      <hr>


      <Section title="Experience">
        <p class="what"><strong>Interaction Design & Photography </strong>&nbsp@ internezzo ag (2017 - 2019)</p>
        <p class="what"><strong>Event Management Internship & Photography </strong>&nbsp@ Küssenberger & Partner (2016 -
          2017)</p>
      </Section>

      <hr>

      <Section title="Education">
        <p class="what"><strong>Interaction Design & Photography </strong>&nbsp@ internezzo ag (2017 - 2019)</p>
        <p class="what"><strong>Event Management Internship & Photography </strong>&nbsp@ Küssenberger & Partner (2016 -
          2017)</p>
      </Section>

      <hr>

      <Section title="Skills">
        <h3>Software</h3>
        <p>Design: Sketch, Figma, Adobe XD, Protopie, Adobe Photoshop, Illustrator, InDesign, Premiere Pro, After Effects</p>
        <p>Code: Basic HTML, CSS and Javascript</p>
        <p>Tools I like: Jira, Confluence, Slack, Bear</p>
      </Section>

      <hr>

      <Section title="Languages">
        <p>Swiss German: Native</p>
        <p>German: Fluent</p>
        <p>English: Fluent</p>
      </Section>
    </div>
  </div>

</template>

<script>

  import headerSection from "../components/headerSection";

  import experience from "../components/experience";

  import Section from "../components/Section";

  import Skill from "../components/Skill";


  export default {
    components: {
      headerSection,
      experience,
      Section,
      Skill
    }
  }

</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Catamaran:300,500,700&display=swap');

  .lead {
    font-family: 'Catamaran', sans-serif;
    font-weight: 300;
    font-size: 1.625rem;
    margin: auto;
    padding-top: 100px;
  }

  .content {
    max-width: 56.875rem;
    margin: 0 auto;
    padding: 15px;
  }

  hr {
    margin: auto;
    margin-top: 6.25rem;
    margin-bottom: 1.5rem;
  }

</style>
