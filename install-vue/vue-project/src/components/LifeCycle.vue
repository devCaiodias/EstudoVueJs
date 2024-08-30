<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default{
        name: 'LifeCycle',
        data() {
            return {
                nome: 'None',
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Caio'
            }, 1000);

            this.lifeCycle()
        },
        mounted () {
            setTimeout(() => {
                this.nome = 'Yuta'

            }, 2000);
            
            this.lifeCycle()
        },
        methods: {
            lifeCycle() {
                console.log('Execultou')
            }
        }
    }
</script>