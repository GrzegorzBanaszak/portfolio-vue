<script lang="ts">
import { defineComponent } from "vue";
import HomeView from "./views/HomeView.vue";
import bgimage from "@/assets/open-bg.jpg";
import Navbar from "@/components/Navbar.vue";

export default defineComponent({
  components: { HomeView, Navbar },
  data() {
    return {
      bg: `url(${bgimage})`,
    };
  },
});
</script>

<template>
  <main class="container" :style="{ backgroundImage: bg }">
    <navbar />
    <router-view></router-view>
  </main>
</template>
