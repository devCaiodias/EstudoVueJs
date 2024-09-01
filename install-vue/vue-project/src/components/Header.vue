<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contatos</a></li>
        <li v-if="esta_logado"><a href="#">Meu perfill</a></li>
    </ul>
</template>

<script>
    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Header',
        props: ["esta_logado"]
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
