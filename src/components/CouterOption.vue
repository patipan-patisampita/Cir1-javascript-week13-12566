<template>
    <div>
        <h2>Vue3 with Optional API</h2>
        <p>{{ count }}</p>
        <button @click="countUp">Count UP</button>
        <button @click="countDown">Count Down</button>
        <button @click="reset">Reset</button>
    </div>
</template>

<script>
export default {
    //1.Optional API
    name: 'CouterOption',
    data() {
        return {
            count:0
        }
    },
    methods: {
        countUp() {
            this.count = this.count + 1
        },
        countDown() {
            this.count = this.count - 1
        },
        reset() {
            this.count = 0
        }
    },
}
</script>

<style lang="scss" scoped>

</style>