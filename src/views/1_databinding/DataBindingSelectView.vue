<template>
  <div>
    <select name="" id="" v-model="selectedCity">
      <option value=""></option>
      <option value="02">서울</option>
      <option value="051">부산</option>
      <option value="064">제주</option>
    </select>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},
  data() {
    return {
      selectedCity: '02'
    }
  },
  methods: {}
})
</script>
