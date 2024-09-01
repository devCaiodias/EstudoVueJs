<template>
    <div>
        <h1>Olá Vue!</h1>
        <p> Meu nome é {{ nome }} </p>
        <p> minha Carreira é {{ Carreira }} </p>
        <MultiplosEventos />
        <Reutilizacao />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue';
    import Reutilizacao from './Reutilizacao.vue';

    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos,
            // eslint-disable-next-line vue/no-unused-components
            Reutilizacao
        },
        data() {
            return {
                nome: "Matheus",
                Carreira: "Dev"
            }
        }
    }
</script>