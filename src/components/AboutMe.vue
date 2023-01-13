<template>
  <div class="greetings">
    <h1 class="green">About Me</h1>
    <h3>
      I'm an enthusiastic, self-motivated, reliable and good team worker.
      <br />
      I love challenging situations because they force me to adapt. I'm able to
      work well in both, team and own initiative environments.
      <br />
      I love motorcycles, BBQ, computers and music but what i will never say no
      to is a good weekend on the beach or the mountain.
    </h3>
  </div>
</template>
  
<style scoped>
h1 {
  font-weight: 500;
  font-size: 1.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
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