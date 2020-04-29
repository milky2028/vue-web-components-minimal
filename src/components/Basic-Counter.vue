<template>
  <div>
    <h2>Basic API Counter</h2>
    <button @click="increment">Increment</button>
    <button @click="decrement">Increment</button>
    <p>Count: {{ count }}</p>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      this.count--;
    },
  },
});
</script>
