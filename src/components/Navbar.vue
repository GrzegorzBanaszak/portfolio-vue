<template>
  <nav class="navbar">
    <div class="navbar-toggle" @click="isShow = !isShow">T</div>
    <transition-group name="links">
      <nav-link v-if="isShow" is :key="1" :title="'About'" :target="'/'"
        ><about-icon></about-icon
      ></nav-link>
      <nav-link v-if="isShow" is :key="2" :title="'Skills'" :target="'/skills'"
        ><tools-icon></tools-icon
      ></nav-link>
      <nav-link
        v-if="isShow"
        is
        :key="3"
        :title="'Projects'"
        :target="'/projects'"
        ><projects-icon></projects-icon
      ></nav-link>
      <nav-link
        v-if="isShow"
        is
        :key="3"
        :title="'Contact'"
        :target="'/contact'"
        ><mail-icon></mail-icon
      ></nav-link>
    </transition-group>
  </nav>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import NavLink from "./NavLink.vue";
import ToolsIcon from "@/icons/ToolsIcon.vue";
import AboutIcon from "@/icons/AboutIcon.vue";
import ProjectsIcon from "@/icons/ProjectsIcon.vue";
import MailIcon from "@/icons/MailIcon.vue";

export default defineComponent({
  components: { NavLink, ToolsIcon, AboutIcon, ProjectsIcon, MailIcon },
  mounted() {
    this.$nextTick(() => {
      window.addEventListener("resize", this.onResize);
    });
  },
  data() {
    return {
      isShow: window.innerWidth > 992,
    };
  },
  methods: {
    onResize() {
      if (window.innerWidth > 992 && this.isShow === false) {
        this.isShow = true;
      }

      if (window.innerWidth < 992 && this.isShow === true) {
        this.isShow = false;
      }
    },
  },
});
</script>
