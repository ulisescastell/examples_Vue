<script setup>
    import { ref } from 'vue'

    const show = ref(false)
</script>

<template>
    <section>
        <h2>Directive v-show example</h2>
        <small>The directive v-show always render contet, but hides it until a condition is true. It has a very similar functionality as the v-if directive</small>
        <br>
        <button @click="show = !show">Show content</button>
    
        <div>
            <p v-show="show">Show variable is now true</p>
        </div>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>