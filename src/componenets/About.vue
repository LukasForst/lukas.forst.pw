<template>
  <div class="about-container">
    <div class="about">
      <p class="about-text md-body-2">
        I'm a motivated and self-driven Software Engineer with in-depth knowledge of Kotlin,
        Software Architecture and passion for functional programming all the way
        from the lambda calculus through Haskell to the Kotlin & JavaScript.
        I love designing and implementing one-click DevOps and have a strong
        experience in architecture design (including PaaS, SaaS) as well as mathematical
        background ranging from group theory, data analysis, AI utilization,
        predictions to mathematical optimization. I have strong experience in software engineering,
        software architecture, client-facing, and leading projects from technical side.
      </p>
      <p class="about-text md-body-2">
        I'm currently pursuing a Cyber Security Master's degree at CTU. I started my career in the
        Prague-based AI startup Blindspot Solutions and then moved to a cybersecurity startup in
        Berlin - Wire. At the beginning of 2020, I co-founded a medical AI startup, Mild Blue,
        where I'm responsible for the products and company security.
        As of 2021, I have four years of experience building production-ready software.
      </p>
    </div>
  </div>

</template>

<script>
export default {
  name: 'About'
};
</script>

<style scoped>
.about-container {
  display: flex;
  justify-content: center;
  padding: 50px;
}

.about {
  /*about-text * 2 + 100px in between*/
  max-width: 1100px;

  display: flex;
  justify-content: space-evenly;
  flex-grow: 1;
  flex-wrap: wrap;
}

.about-text {
  max-width: 500px;
}

p {
  line-height: 2.2;
  font-size: 15px;
  /*noinspection CssFloatPxLength*/
  letter-spacing: .1px;
  text-align: justify;

}
</style>