<template>
  <div class="main">
    <s-button @click="onClick" type="primary">button</s-button>
    <s-input v-model="value" class="input">
      <template #prepend>Http://</template>
    </s-input>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { SButton, SInput } from '@vmkt/shuge-ui'
const value = ref('')
const onClick = () => {
  console.log('click')
}
</script>
<style>
.main {
  width: 300px;
  height: 200px;
}
</style>
