<script lang="ts">
import { defineComponent } from "vue";
import Solar from "@/components/Solar.vue";
import GithubIconVue from "@/icons/GithubIcon.vue";
import LinkedinIconVue from "@/icons/LinkedinIcon.vue";

export default defineComponent({
  components: { Solar, GithubIconVue, LinkedinIconVue },
});
</script>

<template>
  <solar></solar>
  <div class="open-about">
    <h1 class="about-header">About me</h1>
    <ul>
      <li>Hi, I'm Grzegorz Junior Javascript Developer</li>
      <li>I’m interested in football, game and good food</li>
      <li>
        Me free time I spend on reading comics, playing games and polishing me
        programing skills
      </li>
    </ul>
    <div class="about-links">
      <a
        class="about-link github-link"
        href="https://github.com/GrzegorzBanaszak"
        ><github-icon-vue /> github</a
      >
      <a
        class="about-link linkedin-link"
        href="https://github.com/GrzegorzBanaszak"
        ><linkedin-icon-vue />Linkedin</a
      >
    </div>
  </div>
</template>
