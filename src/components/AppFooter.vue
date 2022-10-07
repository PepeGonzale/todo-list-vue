<template>
    <footer>
        <span>Laptop with love &amp; <a href="//vuejs.org">Vue.js</a>in Madrid</span>
    </footer>
</template>
<script>
    export default {
        name: 'app-footer'
    }
</script>
<style lang = "scss">
    footer{
        box-sizing: border-box;
        background-color: #cfd8dc;
        bottom: 0;
        left: 0;
        padding: 1rem;
        position: absolute;
        width: 100%;
            a { 
            text-decoration: none;
            color: #546e7a;
            }
    }
</style>