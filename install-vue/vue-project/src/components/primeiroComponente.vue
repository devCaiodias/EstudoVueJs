<template>
    <div>
        <h1>Olá Vue!</h1>
        <p> Meu nome é {{ nome }} </p>
        <p> minha Carreira é {{ Carreira }} </p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: "Matheus",
                Carreira: "Dev"
            }
        }
    }
</script>