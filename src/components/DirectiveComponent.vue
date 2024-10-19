<script setup>
   const title = 'That\'s a title'
   const imageUrl = 'https://imgs.search.brave.com/_cQjPK4wK8-JqqmacbCofat3zQSAAgNHdBXVGVDNDpE/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9pLnVk/ZW15Y2RuLmNvbS9j/b3Vyc2UvNDgweDI3/MC85OTUwMTZfZWJm/NC5qcGc'
</script>

<template>
    <section>
        <h2>Directive v-bind example</h2>
        <small> The directives let us make our DOM elements and its attributes reactive. So we can modify it through Vue or through the view itself</small>
            <div>
                <h4 v-bind:title="title">Hover your mouse</h4>
                <img v-bind:src="imageUrl" alt="vuelogo" title="vueImg">
            </div>
    </section>
</template>

<style scoped>
    img {
        width: 500px;
        height: 200px;
    }
</style>