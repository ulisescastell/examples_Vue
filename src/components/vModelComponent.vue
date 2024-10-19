<script setup>
    import { ref } from 'vue'

    const userName = ref('')
</script>

<template>
    <section>
        <h2>Directive v-model example</h2>
        <small>The directives v-model makes a bidirectional channel between the view (DOM) and the model (our javascript)</small>
        
        <div>
            <p> The username is: <span> {{ userName }}</span></p>
            <input type="text" v-model="userName" placeholder="Write your username..." />
        </div>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>