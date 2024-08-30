<template>
    <div>
        <p v-if="esta_Trabalhando">Estou Trabalhando no momento.</p>
        <p v-else>Mais Esto estudando no momento.</p>
        <p>Utilizo as seguinte Limguagem: </p>
        <ul>
            <li>Html</li>
            <li>Css</li>
            <li>Js</li>
            <li>Vue</li>
        </ul>
        <p v-show="mostrar_email">Mande essa Mensagem para: {{ email}}</p>
    </div>
</template>

<script>
    export default {
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'info',
        data() {
            return {
                esta_Trabalhando: false,
                mostrar_email: true,
                email: 'caiodias@gmail.com'
            }
        }
    }
</script>