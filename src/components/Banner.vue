<template>
    <div class="banner">
        <h3>{{ msg }}</h3>
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
        padding: 2px;
        background-color: deepskyblue;
        color: white;
        text-align: center;
    }
</style>
