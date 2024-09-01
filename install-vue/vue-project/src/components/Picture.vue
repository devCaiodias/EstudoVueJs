<template>
    <div>
        <img :src="avatar" :alt="descrition" width="200px">
        <Reutilizacao />
    </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue';

    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Picture',
        components: {
            // eslint-disable-next-line vue/no-unused-components
            Reutilizacao,    
        },
        data() {
            return {
                avatar: '/img/best.jpg',
                descrition: 'Vagabond'
            }
        }
    }
</script>