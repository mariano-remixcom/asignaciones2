<template>
  <div class="default-page-wrapper">
    <default-nav />
    <slot />
    <default-footer />
  </div>
</template>

<script setup>
import DefaultFooter from './DefaultFooter.vue'
import DefaultNav from './DefaultNav.vue'
</script>

<style lang="scss">
/* Sticky footer */
html {
  position: relative;
  min-height: 100%;
}
body {
  background-color: $gray-100; /* color de fondo */
  margin-bottom: 60px; /* Margin bottom equal to footer height */
}
.default-page-wrapper {
  padding: 5em 0em 3em 0em;
}
.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 60px; /* Footer height */
  line-height: 60px; /* Vertically center the text */
  background-color: $gray-100;
  text-align: center;
}
</style>
