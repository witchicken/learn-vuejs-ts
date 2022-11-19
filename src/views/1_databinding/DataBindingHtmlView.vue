<template>
  <div>
    <div>{{ htmlString }}</div>
    <div v-html="htmlString"></div>
  </div>
</template>
<script lang="ts">
export default {
  components: {},
  data() {
    return {
      htmlString: '<p style="color:red;">testHtmlString</p>'
    }
  }
}
</script>
