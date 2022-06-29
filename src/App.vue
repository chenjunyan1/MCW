<template>
  <div id="app">

    <h1 style="text-align:center;">computed、methods和watch的区别</h1>

    <!-- <methodsDemo /> -->
    <!--  methods 方法，随着渲染，方法需要被重新调用。遇到一个函数，就从新调用一次 -->


    <!-- <computedDemo /> -->
    <!-- 使用 computed 的好处：提高性能
当我们改变 number 时，整个应用会重新渲染，vue 会被数据重新渲染到 dom 中 -->
    <!-- 而 computed 中的函数所依赖的属性没有发生改变，那么调用当前函数的时候会从缓存中读取，
从而性能开销比较小。当新的值需要大量计算才能得到，缓存的意义就非常大。 -->

    <watchDemo />
    <!-- 只有监听的值发生改变才会改变 -->


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
</style>
