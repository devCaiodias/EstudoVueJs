<template>
    <div>
        <h2>Meu Formulario:</h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <Submit />
        </form>
        <p>Conteudo</p>
    </div>
</template>

<script>
// import InputText from './form/inputText.vue';
import Submit from './form/Submit.vue';

    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Form',
        components: {
            // InputText,
            Submit
        },
        data() {
            return {
                name: '',
                email: ''
            }
        },
        methods: {
            enviarFormulario(e) {
                e.preventDefault();

                const name = this.name
                const email = this.email
                
                console.log(`Dados enviados Nome =${name} e Email =${email}`)

                // Ajax

                // Inserir no banco de dados
            }
        }
    }
</script>