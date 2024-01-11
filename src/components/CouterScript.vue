<template>
    <div>
        <h2>Vue3 with Composition API</h2>
        <p> {{ state.count }}</p>
        <button @click="state.count++">Count Up is:{{ state.count }}</button>
        <button @click="state.count--">Count Down is:{{ state.count }}</button>
        <button @click="state.count = 0 ">Reset:{{ state.count }}</button>
    </div>
</template>

<script setup>
import { ref } from 'vue';

//2.Composition API
//2.2 Script Setup 
const state = ref({ count: 0 })
</script>

<style lang="scss" scoped></style>