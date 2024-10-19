<script setup>
    import { reactive } from 'vue'

    const user = reactive({
        name: 'Ulises',
        age: 19
    })

    const incrementAge = () => user.age++
</script>

<template>
    <section>
        <h2>Reactive example</h2>
        <small>Reactive is used to manage objects or arrays that can change and its values are displayed on the screen</small>
        
        <p>The user <span> {{ user.name }}</span> is <span> {{ user.age }} years old</span> </p>
        <button @click="incrementAge">Increment user age</button>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>