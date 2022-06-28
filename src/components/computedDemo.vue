<template>
  <div>

    <!-- 使用computed方法时不可以加括号，加括号会变成 -->
    <div>Name: {{ name }}</div>
    <div>Name: {{ name }}</div>
    <div>Name: {{ name }}</div>
    <div>Name: {{ name }}</div>
    <div>Name: {{ name }}</div>
    <div>Name: {{ name }}</div>

  </div>
</template>

<script>
export default {
  name: 'computDemo',
  props: {
    msg: String
  },
  data() {
    return {
      firstName: '陈',
      lastName: '俊雁'
    }
  },
  computed: {
    name() {
      console.log("小风车....");
      return `${this.firstName} ${this.lastName}`
    }
  }
}
</script>

<style scoped>
</style>
