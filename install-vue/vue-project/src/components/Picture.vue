<template>
    <img :src="avatar" :alt="descrition" width="200px">
</template>

<script>
    export default {
        // eslint-disable-next-line vue/multi-word-component-names, vue/no-reserved-component-names
        name: 'Picture',
        data() {
            return {
                avatar: '/img/best.jpg',
                descrition: 'Vagabond'
            }
        }
    }
</script>