<template>
    <li>
        <div>
            <header>
                <h3>{{ title }} - {{ author }} - {{ edition }}</h3>
                <button>Supprimer</button>
            </header>
        </div>
        <p>{{ summary }}</p>
        <p>{{ opinion }}</p>
        <a :href="link" target="blank">Voir le résumé en images</a>
    </li>
</template>

<script>
    export default {
        props: ['title', 'auhtor', 'edition', 'summary', 'opinion', 'link']
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

    a {
    text-decoration: none;
    color: #ce5c00;
    }

    a:hover,
    a:active {
    color: #c89300;
    }
    
</style>