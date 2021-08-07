<template>
  <div id="app">
    我的教育
    <h1 @click="d">{{a}}</h1>
    <router-view />
  </div>
</template>
// 需要加 lang="ts"
<script lang="ts">
import Vue from 'vue'
import Component from 'vue-class-component'

// 类的装饰器，用来修饰下面的类；
@Component
export default class App extends Vue {
  // classAPI是当前组件的name属性
  a = 1
  b = '2'
  c = {
    a: 1, b: '2'
  }

  d () {
    console.log(this.a)
    // this.b.abc()
  }

  get name () {
    return this.a + ' ' + this.b
  }

  set name (value) {
    this.b = value + 2
  }

  mounted () {
    console.log('mounted')
    setTimeout(() => {
      console.log(this.name)
    }, 1000)
  }
}
</script>

<style lang="scss" scoped></style>
