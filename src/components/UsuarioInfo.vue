<template>
    <div class="componente">
        <h2>As Informações de Usuário</h2>
        <p>Vários detalhes...</p>
        <p>Nome do usuario : <strong> {{ inverterNome() }} </strong></p>
    </div>
</template>

<script>
export default {
    props: {
        nome: [String]
    },
    methods: {
        inverterNome() {
            return this.nome.split('').reverse().join('')
        }
    },
}
</script>

<style scoped>
    .componente {
        flex: 1;
        background-color: #ec485f;
        color: #fff;
    }
</style>
