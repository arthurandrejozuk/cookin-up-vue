<script lang="ts">
import SelecionarIngrediente from './SelecionarIngrediente.vue';
import SuaLista from './SuaLista.vue';


export default {
    data() {
        return {
            ingredientes: ['Alho', 'Manteiga', 'Orégano']
        }
    },
    components: {
        SelecionarIngrediente,
        SuaLista
    }
};
</script>

<template>
    <main class="conteudo-principal">
        <SuaLista :ingredientes="ingredientes" />
        <SelecionarIngrediente />
    </main>
</template>

<style scoped>
.conteudo-principal {
    padding: 6.5rem 7.5rem;
    border-radius: 3.75rem 3.75rem 0rem 0rem;
    background: var(--creme, #FFFAF3);
    color: var(--cinza, #444);

    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 5rem;
}
</style>