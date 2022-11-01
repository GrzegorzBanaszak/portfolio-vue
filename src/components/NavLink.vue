<template>
  <router-link
    @mouseenter="isShow = true"
    @mouseleave="isShow = false"
    class="navbar-link"
    :to="target"
    ><div class="navbar-icon"><slot></slot></div>
    <transition name="link-description">
      <div v-if="isShow" class="navbar-description">
        {{ title }}
      </div>
    </transition>
  </router-link>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  props: {
    title: {
      type: String,
      required: true,
    },
    target: {
      type: String,
      required: true,
    },
  },
  data() {
    return {
      isShow: false,
    };
  },
});
</script>

<style></style>
