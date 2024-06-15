<script setup lang="ts">
import { ref } from "vue";
import VueHeader from "./components/VueHeader.vue";
import VueLoader from "./components/VueLoader.vue";
const is_loading = ref<Boolean>(false);
</script>

<template>
  <vue-loader v-if="is_loading"></vue-loader>
  <div class="app s-pagewrap ss-home" id="page" v-else>
    <vue-header></vue-header>
  </div>
</template>

<style scoped>
</style>
