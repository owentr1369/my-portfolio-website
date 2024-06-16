<script setup lang="ts">
import { onMounted, ref } from "vue";
import VueHeader from "./components/VueHeader.vue";
import VueLoader from "./components/VueLoader.vue";
import VueIntro from "./components/VueIntro.vue";
import VueAbout from "./components/VueAbout.vue";
const is_loading = ref<Boolean>(false);
onMounted(() => {
  setTimeout(() => {
    document.body.classList.add("ss-show");
  }, 100);
});
</script>

<template>
  <vue-loader v-if="is_loading"></vue-loader>
  <div class="app s-pagewrap ss-home" id="page" v-else>
    <vue-header></vue-header>
    <section id="content" class="s-content">
      <vue-intro></vue-intro>
      <vue-about></vue-about>
    </section>
  </div>
</template>

<style scoped>
</style>
