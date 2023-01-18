<template>
    <h2>Esta é a descrição da pessoa {{ nome }}</h2>
    <Info />
</template>

<script>
    import Info from './info.vue'

    export default {
        name: 'Pessoa',
        components: {
            Info
        },
        data() {
            return {
                nome: 'Daniel'
            }
        }
    }
</script>