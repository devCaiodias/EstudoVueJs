<template>
    <div>
        <p v-if="esta_Trabalhando">Estou Trabalhando no momento.</p>
        <p v-else>Mais Esto estudando no momento.</p>
        <p>Utilizo as seguinte Limguagem para Font-end: </p>
        <ul>
            <li v-for="(linguagem, index) in font_end" v-bind:key="index">{{ linguagem }}</li>
        </ul>
        <p>Utilizo as segintes Limguagem para back-end: </p>
        <ul>
            <li v-for="language in back_end" v-bind:key="language.id">{{ language.limguagem }}</li>
        </ul>
        <div>
            <button @click="showEmail">{{ TextBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande essa Mensagem para: {{ email}}</p>
        <p class="test">Para ver meu portifolio basta <a v-bind:href="meuLink">acessar aki</a></p>
        <Picture/>
    </div>
</template>

<script>
    import Picture from './Picture.vue'
    
    export default {
  // eslint-disable-next-line vue/no-reserved-component-names, vue/no-unused-components
        components: { Picture },
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'info',
        data() {
            return {
                esta_Trabalhando: false,
                mostrar_email: false,
                email: 'caiodias@gmail.com',
                meuLink: 'https://www.lofi.com/',
                TextBotao: 'Mostrar Email',
                font_end: ["html", "css", "vue", "js"],
                back_end: [
                    {id: 1, limguagem: "js"},
                    {id: 2, limguagem: "py"},
                    {id: 3, limguagem: "typeScript"},
                ]
            }
        },
        methods: {
          showEmail() {
            this.mostrar_email = !this.mostrar_email
            
            if (!this.mostrar_email) {
                this.TextBotao = 'Mostrar Email'
            }else {
                this.TextBotao = 'Esconder Email'
            }
          }  
        }
    }
</script>

<style>
    .paragrafo-pai {
        color: blueviolet;
    }
</style>