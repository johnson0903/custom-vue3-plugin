<script setup>
import { ref } from "vue";
const tooltipText = ref("Hello world");
</script>

<template>
  <h1>Custom Vue.js 3 Plugins</h1>
  <input type="text" v-model="tooltipText" /> <br />
  <span
    >Hover Over Me
    <ToolTip :text="tooltipText" :options="{ placement: 'right' }"
  /></span>
</template>
