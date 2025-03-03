<script setup lang="ts">
import ListItem from './ListItem.vue'

</script>
<template>
    <h1>Aufbau der Webseite</h1>
    <ListItem>
    <template #icon>
      Lego
    </template>
    <template #heading>Bausteine</template>
 
    <div class="container">
      <div class="element">
        <p>Das ist ein Textabschnitt</p>
      </div>
      
      <div class="element">
        <button class="button">Login</button>
      </div>
      
      <div class="element">
        <h1>Das ist die Überschrift</h1>
      </div>
      <div class="element">
        <button class="cute-button">Absenden</button>
      </div>
      
      <div class="element">
        <label for="name">Mein Input</label>
        <input type="text" id="name" name="name" class="input" />
      </div>
      <div class="element textblock-bridgerton">
        <h3>Das ist noch eine Überschrift</h3>
      </div>
    </div>
  </ListItem>
</template>
<style scoped>
.container {
  height: 200px;
  background-color: rgb(245, 245, 245);
  border: 1px solid gray;
  border-radius: 5px;
  margin: 24px;
  padding: 24px;
  display: flex;
}

.element {
  margin: 24px;
}
.element:nth-child(even) {
  transform: rotate(5deg);
  margin-top: 12px;
}
.element:nth-child(odd) {
  transform: rotate(-5deg);
  margin-top: 48px;
}


.cute-button {
  background-color: #EA4C89;
  border-radius: 8px;
  border-style: none;
  box-sizing: border-box;
  color: #FFFFFF;
  cursor: pointer;
  display: inline-block;
 } 

 .textblock-bridgerton {
        font-size: 1rem;
        font-family: cursive;
        letter-spacing: 1.5px;
    } 
</style>
