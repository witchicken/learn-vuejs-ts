<template>
  <div>
    <div style="color: red; font-size: 30px">
      스타일 바인딩: 글씨는 red, 폰트크기: 30px
    </div>
    <div :style="style1">스타일 바인딩: 글씨는 red, 폰트크기: 30px</div>
    <button @click="style1.color = 'blue'">색바꾸끼</button>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},
  data() {
    return {
      style1: {
        color: 'green',
        fontSize: '30px'
      }
    }
  },
  methods: {}
})
</script>
