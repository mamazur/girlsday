<script setup lang="ts">
import ListItem from './ListItem.vue'
import CopyBlock from '../components/CopyBlock.vue'

</script>

<template>
  <h1>HTML Elemente</h1>
  <ListItem>
    <template #icon>
      HTML
    </template>
    <template #heading>Überschrift und Text</template>
    <CopyBlock :htmlCode="`
  <div>
    <h1>Das ist die Überschrift</h1>
    <p>Das ist ein Textabschnitt</p>
  </div>
`"></CopyBlock>
  </ListItem>

  <ListItem>
    <template #icon>
      HTML
    </template>
    <template #heading>Input</template>

    <CopyBlock :htmlCode="`
    <div>
      <label for='name'>Mein Input</label>
      <input type='text' id='name' name='name' class='input' />
    </div>
      `">
    </CopyBlock>
  </ListItem>

  <ListItem>
    <template #icon>
      HTML
    </template>
    <template #heading>Button</template>
    <CopyBlock :htmlCode="`
    <div>
      <button class='button'>Login</button>
    </div>
      `">
    </CopyBlock>
  </ListItem>

  <ListItem>
    <template #icon>
      HTML
    </template>
    <template #heading>Image</template>
    <CopyBlock :htmlCode="`
    <div>
      <image src='beispiel-bild.jpg' />
    </div>
    `">
    </CopyBlock>
  </ListItem>

</template>
