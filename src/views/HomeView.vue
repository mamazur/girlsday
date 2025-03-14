<script setup lang="ts">
import StyleList from '../components/StyleList.vue'
import ElementList from '../components/ElementList.vue'
import Glowing from '../components/Glowing.vue'
import LegoElements from '../components/LegoElements.vue'
</script>

<template>
  <img src="../../public/logo.jpg" />
  <main>
    <LegoElements></LegoElements>
    <ElementList />
    <Glowing></Glowing>
    <StyleList />
    <Glowing></Glowing>
  </main>
</template>
<style scoped>
main {
  min-height: 100vh;
}
</style>
