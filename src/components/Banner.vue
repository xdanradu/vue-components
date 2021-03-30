<template>
    <div class="banner">
        <h1>{{ msg }}</h1>
        <slot></slot>
    </div>
</template>
<script>
    export default {
        name: 'Banner',
        props: {
            msg: String,
        }
    };
</script>
<style scoped>
    .banner {
        padding: 12px;
        background-color: #fcf6cd;
        color: #f6a623;
        text-align: left;
        position: fixed;
        z-index: 2;
    }
</style>
