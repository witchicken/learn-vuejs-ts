<template>
  <div>
    <div :class="{ 'text-red': hasError, active: isActive }">클래스 바인딩</div>
    <button @click="changeCss">true/false</button>
    <div :class="class2">클래스 바인딩2</div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},
  data() {
    return {
      isActive: false,
      hasError: true,
      class2: ['active', 'hasError']
    }
  },
  methods: {
    changeCss() {
      this.isActive = !this.isActive
    }
  }
})
</script>
<style scoped>
.active {
  background-color: greenyellow;
  font-weight: bold;
}
.text-red {
  color: red;
}
</style>
