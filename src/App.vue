<script setup>
  import { ref } from "vue";

  const count = ref(0);
</script>

<template>
  <div>
    <h3>
      The current count is 
    </h3>
    <h1 class="text-center">
      {{count}}
    </h1>
    <button class="btn red-background white-text" @click="count--">-</button>
    <button class="btn green-background white-text" @click="count++">+</button>
  </div>
</template>