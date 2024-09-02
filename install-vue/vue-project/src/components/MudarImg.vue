<template>
    <div>
        <button @click="$emit('mudarimagem')">Trocar img</button>
    </div>
</template>

<script>
    export default {
        name: 'MudarImg',
        emits: ['mudarimagem']
    }
</script>