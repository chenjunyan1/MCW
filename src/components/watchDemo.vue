<template >
    <div>

        <h1>watch Demo:</h1>

        <input v-model="numData" type="number" step="1" />
        <h1>{{ numData }}</h1>
        <button @click="helle">button</button>

    </div>
</template>
<script>
export default {
    name: 'watchDemo',
    data() {
        return {
            numData: 0,
        }
    },
    methods: {
        helle(){
            this.numData = 9;
            console.log("helle");
        }
    },
    watch: {
        // 当需要监听一个对象的改变时，普通的watch方法无法监听到对象内部属性的改变，
        // 只有data中的数据才能够监听到变化，此时就需要deep属性对对象进行深度监听。
        numData(newVal, oldVal) {
            console.log(newVal,oldVal+"+++");
            console.log("aaaaa");
        }

    }
}
</script>
<style >
</style>