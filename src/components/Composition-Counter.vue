<template>
  <div>
    <h2>Composition API Counter</h2>
    <button @click="increment">Increment</button>
    <button @click="decrement">Increment</button>
    <p>Count: {{ count }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from "@vue/composition-api";
export default defineComponent({
  setup() {
    const count = ref(0);

    const increment = () => count.value++;
    const decrement = () => count.value--;

    return {
      count,
      increment,
      decrement,
    };
  },
});
</script>
