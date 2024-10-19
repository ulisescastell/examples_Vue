<script setup>
    import { ref } from 'vue'

    const counter = ref(0)

    const incrementCounter = () => counter.value++
</script>

<template>
    <section>
        <h2>Ref example</h2>
        <small>Ref is used to manage primitive values that can change as numbers or strings and are displayed on the screen</small>
        
        <p>Counter value: {{ counter }}</p>
        <button @click="incrementCounter">Increment</button>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>