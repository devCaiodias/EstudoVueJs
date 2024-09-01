<template>
    <div>
        <h2>Essa é a descriçao da pessoa: {{ nome }}</h2>
        <info  :email="email" :esta_Trabalhando="esta_Trabalhando"/>
        <Form/>
    </div>
</template>

<script>
import Form from './form.vue';
import info from './info.vue'
    export default {
    components: { 
        info,
        // eslint-disable-next-line vue/no-reserved-component-names
        Form
    },
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'Pessoa',
        data() {
            return {
                nome: 'Caio',
                email: 'caiodias22@gmail.com',
                esta_Trabalhando: true

            }
        }
    }
</script>