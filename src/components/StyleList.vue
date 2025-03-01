<script setup lang="ts">
import ListItem from './ListItem.vue'
import CopyBlock from '../components/CopyBlock.vue'

</script>

<template>
  <ListItem addColor>
    <template #icon>
      CSS
    </template>
    <template #heading>Textblock Modern</template>
    <CopyBlock :htmlCode="`
      .textblock-modern {
          font-size: 1rem;
          font-family: 'Gill Sans', sans-serif; letter-spacing: 1px; 
      } `" addColor></CopyBlock>
  </ListItem>
  <ListItem addColor>
    <template #icon>
      CSS
    </template>
    <template #heading>Textblock Bridgerton</template>
    <CopyBlock :htmlCode="`
      .textblock-bridgerton {
          font-size: 1rem;
          font-family: cursive;
          letter-spacing: 1.5px;
      } `" addColor></CopyBlock>
  </ListItem>
  <ListItem addColor>
    <template #icon>
      CSS
    </template>
    <template #heading>Modern Input</template>
    <CopyBlock :htmlCode="`
    .modern-input {
        width: 95%;
        background-color: rgba(0, 144, 255, 0.05);
        padding: 12px 15px;
        border-color: #007BFF;
        border: 2px solid #ccc;
        border-radius: 5px;
        outline: none;
      } `" addColor></CopyBlock>
  </ListItem>
  <ListItem addColor>
    <template #icon>
      CSS
    </template>
    <template #heading>Cute Button</template>
    <CopyBlock :htmlCode="`
 
.cute-button {
  background-color: #EA4C89;
  border-radius: 8px;
  border-style: none;
  box-sizing: border-box;
  color: #FFFFFF;
  cursor: pointer;
  display: inline-block;
 } `" addColor></CopyBlock>
  </ListItem>

</template>
