<script setup>
    const cars = [
        { 
            id: 1,
            brand: "ferrari",
            price: 1000090 
        },
        {
            id: 2,
            brand: "lamborghini",
            price: 3010090 
        },
        {
            id: 3,
            brand: "renault",
            price: 14700
        }

    ]
</script>

<template>
    <section>
        <h2>Directive v-for example</h2>
        <small>The directive v-for is used to render arrays in the DOM</small>
        <ul>
            <li v-for="car in cars" :key="car.id">Car brand: {{ car.brand }} - Car price: {{ car.price }}</li>
        </ul>
    </section>
</template>

<style scoped>
    span {
        font-weight: bold;
    }
</style>