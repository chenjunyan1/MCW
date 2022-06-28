<template>
  <div id="app">
    <!-- <computedDemo /> -->

    <!-- 使用 computed 的好处：提高性能
当我们改变 number 时，整个应用会重新渲染，vue 会被数据重新渲染到 dom 中 -->




    <!-- <methodsDemo /> -->
    <!--  methods 方法，随着渲染，方法需要被重新调用。遇到一个函数，就从新调用一次 -->

    <watchDemo />


  </div>
</template>

<script>

import computedDemo from './components/computedDemo.vue'
import methodsDemo from './components/methodsDemo.vue'
import watchDemo from './components/watchDemo.vue'
export default {
  name: 'app',
  components: {
    computedDemo,
    methodsDemo,
    watchDemo
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
