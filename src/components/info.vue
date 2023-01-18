<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>HTML</li>
            <li>CSS</li>
        </ul>
        <p v-show="mostrar_email">Mande um email para: {{ email }}</p>
        <p>Para acessar meu portifólio acesse o <a v-bind:href="meu_link">link</a></p>
    </div>
</template>

<script lang="ts">
    export default {
        name: 'Info',
        data() {
            return {
                esta_trabalhando: false,
                mostrar_email: false,
                email: 'dnddan79@gmail.com',
                meu_link: 'https://google.com'
            }
        }
    }
</script>