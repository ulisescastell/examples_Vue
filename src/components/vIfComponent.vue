<script setup>
    import { ref } from 'vue'

    const isLogged = ref(false)
    const logIn = () =>  { isLogged.value = true }
    const logOut = () =>  { isLogged.value = false }
</script>

<template>
    <section>
        <h2>Directive v-if example</h2>
        <small>The directive v-if renders its content based on a condiiton. It help us to make conditional rendering</small>
        <p v-if="isLogged">Welcome user!</p>
        <p v-else>Log in, please</p>
        <button v-if="!isLogged" @click="logIn">Log in</button>
        <button v-if="isLogged" @click="logOut">Log out</button>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>