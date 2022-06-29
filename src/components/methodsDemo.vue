<template >
    <div>
        <h1>methods Demo:</h1>
        <div>Name: {{ name() }}</div>
        <div>Name: {{ name() }}</div>
        <div>Name: {{ name() }}</div>
        <div>Name: {{ name() }}</div>
        <div>Name: {{ name() }}</div>
        <div>Name: {{ name() }}</div>
    </div>
</template>
<script>
export default {
    name: 'methodsDemo',
    props: {
        msg: String
    },
    data() {
        return {
            firstName: '陈',
            lastName: '俊雁'
        }
    },
    methods: {
        name() {
            console.log("小风车....");
            return `${this.firstName} ${this.lastName}`
        }
    }
}
</script>
<style >
</style>