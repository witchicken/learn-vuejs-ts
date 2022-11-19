<template>
  <div>
    <div>
      <select name="" id="">
        <option :value="city.code" :key="city.code" v-for="city in cities">
          {{ city.title }}
        </option>
      </select>
    </div>
  </div>
  //2:57
</template>
<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  components: {},
  data() {
    return {
      cities: [
        { title: '서울', code: '02' },
        { title: '부산', code: '051' },
        { title: '광주', code: '062' }
      ],
      drinkList: [
        { drinkId: '1', drinkName: '코카콜라', price: 700, qty: 4 },
        { drinkId: '2', drinkName: '사이다', price: 800, qty: 2 },
        { drinkId: '3', drinkName: '환타', price: 500, qty: 3 },
        { drinkId: '4', drinkName: '웰치스', price: 600, qty: 6 },
        { drinkId: '5', drinkName: '암바사', price: 800, qty: 10 },
        { drinkId: '6', drinkName: 'TOP', price: 1000, qty: 12 }
      ]
    }
  },

  methods: {}
})
</script>
