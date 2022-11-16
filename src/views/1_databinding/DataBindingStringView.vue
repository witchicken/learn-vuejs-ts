<template>
  <div>
    <h1 class="text-red">Hello {{ userName }}</h1>
    <p>{{ message }}</p>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    return {
      userName: 'John Doe',
      message: 'message Test',
      arr: [],
      obj: {}
    }
  }
}
</script>
<style scoped>
.text-red {
  color: red;
}
</style>
