<script lang="ts">
import { defineComponent } from "vue";
import HomeView from "./views/HomeView.vue";
import bgimage from "@/assets/open-bg.jpg";

export default defineComponent({
  components: { HomeView },
  data() {
    return {
      bg: `url(${bgimage})`,
    };
  },
});
</script>

<template>
  <main class="open" :style="{ backgroundImage: bg }">
    <router-view></router-view>
  </main>
</template>
