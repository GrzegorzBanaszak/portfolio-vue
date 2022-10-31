<template>
  <div class="solar-system">
    <div class="sun"><tools-icon-vue /></div>
    <div class="box">
      <div class="orbit orbit-3">
        <div class="icon redux"><redux-icon-vue /></div>
        <div class="icon nest"><nest-icon-vue /></div>
        <div class="icon figma"><figma-icon-vue /></div>
        <div class="icon mongodb"><mongodb-icon-vue /></div>
        <div class="icon firebase"><firebase-icon-vue /></div>
        <div class="icon git"><git-icon-vue /></div>
        <div class="icon github"><github-icon-vue /></div>
        <div class="icon vscode">
          <visual-studio-code-icon-vue />
        </div>
      </div>
      <div class="orbit orbit-1">
        <div class="icon typescript"><typescript-icon-vue /></div>
        <div class="icon react"><react-icon-vue /></div>
        <div class="icon node"><node-icon-vue /></div>
        <div class="icon vue"><vue-icon-vue /></div>
      </div>
      <div class="orbit orbit-2">
        <div class="icon html"><html-icon-vue /></div>
        <div class="icon css"><css-icon-vue /></div>
        <div class="icon sass"><sass-icon-vue /></div>
        <div class="icon javacript">
          <javascript-icon-vue />
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import JavascriptIconVue from "@/icons/JavascriptIcon.vue";
import TypescriptIconVue from "@/icons/TypescriptIcon.vue";
import HtmlIconVue from "@/icons/HtmlIcov.vue";
import CssIconVue from "@/icons/CssIcon.vue";
import SassIconVue from "@/icons/SassIcon.vue";
import ReactIconVue from "@/icons/ReactIcon.vue";
import VueIconVue from "@/icons/VueIcon.vue";
import ReduxIconVue from "@/icons/ReduxIcon.vue";
import NodeIconVue from "@/icons/NodeIcon.vue";
import NestIconVue from "@/icons/NestIcon.vue";
import FigmaIconVue from "@/icons/FigmaIcon.vue";
import MongodbIconVue from "@/icons/MongodbIcon.vue";
import FirebaseIconVue from "@/icons/FirebaseIcon.vue";
import GitIconVue from "@/icons/GitIcon.vue";
import GithubIconVue from "@/icons/GithubIcon.vue";
import VisualStudioCodeIconVue from "@/icons/VisualStudioCodeIcon.vue";
import ToolsIconVue from "@/icons/ToolsIcon.vue";

export default defineComponent({
  components: {
    JavascriptIconVue,
    TypescriptIconVue,
    HtmlIconVue,
    CssIconVue,
    SassIconVue,
    ReactIconVue,
    VueIconVue,
    ReduxIconVue,
    NodeIconVue,
    NestIconVue,
    FigmaIconVue,
    MongodbIconVue,
    FirebaseIconVue,
    GitIconVue,
    GithubIconVue,
    VisualStudioCodeIconVue,
    ToolsIconVue,
  },
  methods: {
    hello(text: string) {
      console.log(text);
    },
  },
});
</script>
