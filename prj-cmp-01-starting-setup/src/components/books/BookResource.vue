<template>
    <base-card>
        <li>
            <div>
                <header>
                    <h3>{{ title }} - {{ author }} - {{ edition }}</h3>
                    <button>Supprimer</button>
                </header>
            </div>
            <p><span>Résumé</span> - {{ summary }}</p>
            <p><span>Avis</span> - {{ opinion }}</p>
            <a :href="link" target="blank">Voir le résumé en images</a>
        </li>    
    </base-card>
    
</template>

<script>
    
    export default {
        props: ['title', 'author', 'edition', 'summary', 'opinion', 'link']
    }
</script>

<style scoped>

    li {
    margin: auto;
    max-width: 40rem;
    }

    header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    }

    h3 {
    font-size: 1.25rem;
    margin: 0.5rem 0;
    }

    p {
    margin: 0.5rem 0;
    }

    p span{
        color: #c89300;
        font-size: 1.2rem;
    }

    a {
    text-decoration: none;
    color: #ce5c00;
    }

    a:hover,
    a:active {
    color: #c89300;
    }
    
</style>