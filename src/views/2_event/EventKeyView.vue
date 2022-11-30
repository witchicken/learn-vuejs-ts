<template>
  <div>
    <!--<input
      type="search"
      name=""
      id=""
      v-model="searchText"
      @keyup="checkEnter($event)"
    />-->
    <input
      type="search"
      name=""
      id=""
      @keyup.enter="doSearch"
      v-model="searchText"
    />
    <button @click="doSearch">조회</button>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
interface State {
  searchText: string
}
export default defineComponent({
  components: {},
  data(): State {
    return {
      searchText: ''
    }
  },
  methods: {
    doSearch() {
      console.log(this.searchText)
      this.searchText = ''
    },
    checkEnter(event: any) {
      if (event.keyCode === 13) {
        this.doSearch()
      }
    }
  }
})
</script>
