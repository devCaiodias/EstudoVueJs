<template>
    <div>
        <h1>Olá Vue!</h1>
        <p> Meu nome é {{ nome }} </p>
        <p> minha Carreira é {{ Carreira }} </p>
        <MultiplosEventos />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue'

    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos
        },
        data() {
            return {
                nome: "Matheus",
                Carreira: "Dev"
            }
        }
    }
</script>