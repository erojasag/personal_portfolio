<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Know more about my
      <a href="https://github.com/erojasag" target="_blank" rel="noopener"
        >Github</a
      >
      projects and profesional carreer on
      <a
        href="https://www.linkedin.com/in/emanuel-rojas/"
        target="_blank"
        rel="noopener"
        >LinkedIn</a
      >.
    </h3>
    <h4 id="cv">
      <a href="../assets/Emanuel_Rojas Aguero_CV.pdf" download
        >Download My CV 🚀</a
      >
    </h4>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}
#cv {
  padding-top: 20px;
  padding-left: 40px;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
