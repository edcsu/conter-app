<script setup>
import { ref } from "vue";

const count = ref(0);

const addToCount = () => {
  count.value++
}

const subtractFromCount = () => {
  count.value--
}

</script>

<template>
  <main>
    <div>
      <h3>
        The current count is
      </h3>
      <h1 class="text-center">
        {{ count }}
      </h1>
      <button class="btn red-background white-text" @click="subtractFromCount">-</button>
      <button class="btn green-background white-text" @click="addToCount">+</button>
    </div>
  </main>
</template>