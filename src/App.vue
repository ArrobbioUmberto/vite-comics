<script setup>
// import HelloWorld from './components/HelloWorld.vue'
import ComicsHeader from './components/ComicsHeader.vue';
import ComicsMain from './components/ComicsMain.vue';
import ComicsFooter from './components/ComicsFooter.vue';
</script>

<template>
  <ComicsHeader></ComicsHeader>
  <ComicsMain></ComicsMain>
  <ComicsFooter></ComicsFooter>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
