<template>
  <div id="app">
    <router-view />
  </div>
</template>
// 需要加 lang="ts"
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      a: 1,
      b: '2'
    }
  },
  methods: {
    test () {
      // this.b.abc()
    }
  }
})
</script>

<style lang="scss" scoped>
// @import '~@/styles/variables.scss';
.text {
  color: $danger-color;
}

</style>
