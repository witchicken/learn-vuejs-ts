<template>
  <div>
    <div>
      <select name="" id="">
        <option :value="city.code" :key="city.code" v-for="city in cities">
          {{ city.title }}
        </option>
      </select>
    </div>
    <div>
      <table>
        <thead>
          <tr>
            <th>제품번호</th>
            <th>제품명</th>
            <th>가격</th>
            <th>주문수량</th>
            <th>합계</th>
          </tr>
        </thead>
        <tbody>
          <tr :key="drink.drinkId" v-for="drink in drinkList">
            <td>{{ drink.drinkId }}</td>
            <td>{{ drink.drinkName }}</td>
            <td>{{ drink.price }}</td>
            <td><input type="number" name="" id="" v-model="drink.qty" /></td>
            <td>{{ drink.qty * drink.price }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
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
