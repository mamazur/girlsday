<script setup lang="ts">
import StyleList from '../components/StyleList.vue'
import ElementList from '../components/ElementList.vue'
import Glowing from '../components/Glowing.vue'
import LegoElements from '../components/LegoElements.vue';
</script>

<template>
  <img src="../../public/logo.jpg" />
  <main>
    <Glowing></Glowing>
    <LegoElements></LegoElements>
    <Glowing></Glowing>
    <ElementList />
    <Glowing></Glowing>
    <Glowing></Glowing>
    <StyleList />
  </main>
</template>
<style scoped>
main {
  min-height: 100vh;
}
</style>
