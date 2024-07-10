<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="() => {
  if(count > 10){
    count = 0;
  } else {
    count++;
  }}">count is {{ count }}</button>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
