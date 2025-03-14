<script setup lang="ts">
import ListItem from './ListItem.vue'
import CopyBlock from '../components/CopyBlock.vue'
</script>

<template>
  <h1>CSS Klassen</h1>
  <ListItem addColor="lilac">
    <template #icon> CSS </template>
    <template #heading>Textblock Modern</template>
    <CopyBlock
      :htmlCode="`
    .textblock-modern {
        font-size: 16px;
        font-family: 'Gill Sans', sans-serif; letter-spacing: 1px; 
    }`"
      addColor="lilac"
    ></CopyBlock>
  </ListItem>
  <ListItem addColor="lilac">
    <template #icon> CSS </template>
    <template #heading>Textblock Bridgerton</template>
    <CopyBlock
      :htmlCode="`
    .textblock-bridgerton {
        font-size: 16px;
        font-family: cursive;
        letter-spacing: 1.5px;
    } `"
      addColor="lilac"
    ></CopyBlock>
  </ListItem>
  <ListItem addColor="lilac">
    <template #icon> CSS </template>
    <template #heading>Modern Input</template>
    <CopyBlock
      :htmlCode="`
    .modern-input {
        background-color: pink;
        padding: 12px 15px;
        border-color: gray;
        border: 2px solid #ccc;
        border-radius: 5px;
        outline: none;
      } `"
      addColor="lilac"
    ></CopyBlock>
  </ListItem>
  <ListItem addColor="lilac">
    <template #icon> CSS </template>
    <template #heading>Cute Button</template>
    <CopyBlock
      :htmlCode="`
.cute-button {
  background-color: pink;
  border-radius: 8px;
  border-style: none;
  box-sizing: border-box;
  color: white;
  cursor: pointer;
  display: inline-block;
 } `"
      addColor="lilac"
    ></CopyBlock>
  </ListItem>
</template>
