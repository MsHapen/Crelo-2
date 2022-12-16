<script setup>
import HeaderComp from "../src/components/HeaderComp.vue";
</script>
<template>
  <HeaderComp />
  <main>
    <RouterView />
  </main>
</template>
<style>
body {
  margin: 0;
}
main {
  padding: 1%;
}
</style>
