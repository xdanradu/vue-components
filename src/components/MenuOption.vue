<template>
        <div>
            <a :href="url">{{ option }}</a>
        </div>
</template>
<script>
    export default {
        name: 'MenuOption',
        props: {
            url: String,
            option: String
        }
    };
</script>
<style scoped>
    div {
        display: inline-block;
        padding: 0;
        margin-right: 35px;
        line-height: 0.8em;
    }

    a {
        font-weight: 400;
        font-size: 20px;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-align: center;
        -ms-flex-align: center;
        align-items: center;
        white-space: nowrap;
        position: relative;
        padding: 9px 0;
        text-decoration: none;
        color: #F0C34E;
    }
    a::before {
        content: '';
        left: 0;
        bottom: 0;
        height: 1px;
        width: 0;
        background: #b9bbbe;
        position: absolute;
        transition: all .5s;
        top: auto;
        transform: none;
        z-index: -1;
        opacity: 1;
    }

    a:hover::before {
        width: 100%;
    }

    a::after {
        content: '';
        right: 0;
        top: 0;
        height: 1px;
        width: 0;
        background: #b9bbbe;
        position: absolute;
        transition: all .5s;
        bottom: auto;
        transform: none;
        z-index: -1;
        opacity: 1;
    }

    a:hover::after {
        width: 100%;
    }
</style>
