<template>
    <div>
        <button @click="primeiro(txt1,$event), segundo(txt2, $event), terceiro($event)">Ativar multipos Eventos</button>
        <p>{{ multiplos_event }}</p>
    </div>
</template>


<script>
    export default {
        name: 'MultiplosEventos',
        data() {
            return {
                multiplos_event: '',
                txt1: 'Primeiro evento',
                txt2: 'Segundo evento'
            }
        },
        methods: {
            primeiro(txt) {
                this.multiplos_event = txt
            },

            segundo(txt) {
                setTimeout(() => this.multiplos_event = txt, 2000)
            },
            terceiro() {
                setTimeout(() => this.multiplos_event = "", 3000)
            }
        }
    }
    
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>