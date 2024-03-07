<template>
    <div class="commande">
        <h2>Liste des commandes</h2>
        <p>{{ myProp }}</p>
    </div>
</template>

<script>
export default {
    props: {
        myProp: {
            type: String,
            default: 'Voici les commandes en cours :'
        }
    },
    created() {
        this.fetchCommands();
    },
    methods: {
        async fetchCommands() {
            try {
                const response = await fetch('http://localhost:3000/commande');
                const data = await response.json();
                console.log(data);
            } catch (error) {
                console.error(error);
            }
        }
    }
}
</script>

<style scoped>
/* Vos styles CSS ici */
</style>
