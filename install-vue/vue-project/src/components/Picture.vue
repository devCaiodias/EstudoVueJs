<template>
    <div>
        <img :src="avatar" :alt="descrition" width="200px">
        <MudarImg @mudarimagem="trocarimg" />
    </div>
</template>

<script>
    import MudarImg from './MudarImg.vue';

    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Picture',
        components: {
            // eslint-disable-next-line vue/no-unused-components
            MudarImg 
        },
        data() {
            return {
                avatar: '/img/best.jpg',
                descrition: 'Vagabond'
            }
        },
        methods: {
            trocarimg() {
                this.avatar = '/img/best2.jpg'
                console.log('Oi')
            }
        }
    }
</script>