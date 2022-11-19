<template>
  <div>
    <input type="text" v-model="userId" />
    <button @click="myFunction">클릭</button>
    <button @click="changeData">변경</button>
    <br />
    <input type="text" v-model="num1" /> +
    <input type="text" v-model="num2" /> =
    <div>{{ num1 + num2 }}</div>
    <br />
    <input type="text" v-model.number="num3" /> +
    <input type="text" v-model.number="num4" /> =
    <div>{{ num3 + num4 }}</div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},

  data() {
    return {
      userId: 'enigkim.go',
      num1: 0,
      num2: 0,
      num3: 0,
      num4: 0
    }
  },
  methods: {
    myFunction() {
      console.log(this.userId)
    },
    changeData() {
      this.userId = 'test123'
    }
  }
})
</script>
