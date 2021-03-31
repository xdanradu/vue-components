<template>
    <div class="card">
        <h1>My Vue Web Component</h1>
        <div @click="onClickButton($event)" class="message">{{ msg }}</div>
    </div>
</template>
<script>
    export default {
        emits: ['divclicked'],
        props: ['msg'],
        methods: {
            onClickButton () {
                console.log('clicked in child');
                const message = 'some message from the component';
                this.$emit('divclicked', 'submit', { message })
            }
        }
    }
</script>

<style scoped>
    .card {
        font-family: 'Roboto', sans-serif;
        color: crimson;
        text-underline: crimson;
    }
    .message {
        background-color: cornflowerblue;
        color: white;
    }

</style>
