<template>
    <div>
        <button @click="$emit('changeImage')">Alterar Imagem</button>
    </div>
</template>

<script>
export default {
    name: 'ChangeImage',
    emits: ['changeImage']
}
</script>

<style scoped>
button {
    display: flex;
    margin: auto;
}
</style>