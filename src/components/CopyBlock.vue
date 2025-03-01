<script setup lang="ts">
import { ref } from 'vue';

const props = defineProps<{ htmlCode: string, addColor?: boolean }>()
const copied = ref(false);
const codeBlock = ref(null);

const copyToClipboard = async () => {
  try {
    await navigator.clipboard.writeText(props.htmlCode);
    copied.value = true;
    setTimeout(() => (copied.value = false), 2000);
  } catch (err) {
    console.error('Failed to copy:', err);
  }
};
</script>
<template>
  <div class="code-block" :class="{ color: addColor }">
    <pre><code ref="codeBlock">{{ htmlCode }}</code></pre>
    <button @click="copyToClipboard" class="copy-button">
      {{ copied ? "Copied!" : "Copy" }}
    </button>
  </div>
</template>
<style scoped>
.code-block {
  position: relative;
  background-color: rgb(245, 245, 245);
  border: 1px solid gray;
  border-radius: 5px;
  margin: 24px;
  padding: 24px;
}
 
.copy-button {
  right: 0;
  top: 0;
  position: absolute;
  margin: 24px;
}

.color {
  background-color: rgb(242, 231, 255);
  border: 1px solid rgb(197, 149, 255);
}
</style>
