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