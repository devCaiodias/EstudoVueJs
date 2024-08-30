<template>
    <div>
        <h2>Meu Formulario:</h2>
        <form action="">
            <div>
                <InputText />
            </div>
            <div>
                <InputText />
            </div>
            <Submit />
        </form>
    </div>
</template>

<script>
import InputText from './form/inputText.vue';
import Submit from './form/Submit.vue';

    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Form',
        components: {
            InputText,
            Submit
        }
    }
</script>