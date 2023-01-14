<script setup>
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import SupportIcon from "./icons/IconSupport.vue";
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Biography</template>
    Born and raised in Alajuela, Costa Rica<br />
    Emanuel, is a 24 years old software engineer that is passionate about web
    development and building aplications that will have impact in the users
    day-to-day.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Development Stack</template>

    <a href="https://www.mongodb.com/" target="_blank" rel="noopener"
      >MongoDB</a
    >
    <br />
    <a href="https://expressjs.com/" target="_blank" rel="noopener"
      >Express.js</a
    >
    <br />
    <a href="https://angularjs.org/" target="_blank" rel="noopener"
      >AngularJS</a
    >
    <br />
    <a href="https://nodejs.org/" target="_blank" rel="noopener">Nodejs</a>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Contact</template>

    Email:
    <a href="mailto:emanuel@emanuelrojas.com" target="_blank" rel="noopener"
      >emanuel@emanuelrojas.com</a
    >
    <br />
    Phone: +506 8866-7456
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Follow Me</template>

    I have presence on
    <a
      href="https://www.instagram.com/merakiema.dev/"
      target="_blank"
      rel="noopener"
      >Instagram</a
    >
    |
    <a href="https://twitter.com/merakiema_dev" target="_blank" rel="noopener"
      >Twitter</a
    >
  </WelcomeItem>
  
</template>
