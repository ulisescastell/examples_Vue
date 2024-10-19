<script setup>
    import {ref, computed} from 'vue'

    const name = ref('ulises')
    const upperName = computed(() => name.value.toUpperCase())
</script>

<template>
    <section>
        <h2>Computed example</h2>
        <small> Computed makes dynamics variables. </small>
        <div>
            <p>The value is <span>{{ name }}</span> and the computed value is <span>{{ upperName }}</span></p>
        </div>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>