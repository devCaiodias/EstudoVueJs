<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contatos</a></li>
    </ul>
</template>

<script>
    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Header'
    }
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
    }
    
    li {
        margin-right: 10px;
    }

    a {
        text-decoration: none;
        color: aqua;
    }
</style>
