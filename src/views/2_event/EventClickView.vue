<template>
  <div>
    <button @click="increaseCounter">Add 1</button>
    <button @click="decreaseCounter">Minus 1</button>

    <p>{{ counter }}</p>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},
  data() {
    return {
      counter: 0
    }
  },

  methods: {
    increaseCounter() {
      this.counter++
    },
    decreaseCounter() {
      this.counter--
    }
  }
})
</script>
