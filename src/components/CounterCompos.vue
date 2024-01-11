<template>
    <div>
        <h2>Vue3 with Composition API</h2>
        <h2>{{ count }}</h2>
        <button @click="countUp">Counter Up</button>
        <button @click="countDown">Counter Down</button>
        <button @click="reset">Reset</button>
    </div>
</template>

<script>
import { ref } from 'vue'

export default {
    //2.Composition API
    //2.1 Setup option
    setup() {
        const count = ref(0)
        function countUp() {
            count.value = count.value + 1
        }

        function countDown() {
            count.value = count.value - 1
        }

        function reset() {
            count.value = 0
        }

        return { count, countUp, countDown, reset }
    }
}
</script>

<style lang="scss" scoped></style>