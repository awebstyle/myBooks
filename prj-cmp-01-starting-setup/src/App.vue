<template>
    <h1>Dernières lectures</h1>
    <ul>
        <li v-for="storedBook in storedBooks" :key="storedBook.id">
            <h2>{{ storedBook.title }}</h2>
            <h3>{{ storedBook.author }} - {{ storedBook.edition }}</h3>
            <p>Résumé : {{ storedBook.summary }}</p>
            <p>Avis : {{ storedBook.opinion }}</p>
        </li>
    </ul>
</template>

<script>
    export default {
        data(){
            return {
                storedBooks: [
                {
                    id: 'clStendhalRN',
                    title: 'le rouge et le noir',
                    author: 'Stendhal',
                    edition: 'Les Cent Chefs-d\'oeuvre',
                    summary: 'Julien Sorel, fils de charpentier, doté de capacités intellectuelles supérieurs, tente de s\'élever dans la société. Passionné par Napoléon, il rêve d\'une grande destinée en revêtant l\'habit de soldat (rouge) mais c\'est celui du clergé (noir) qu\'il sera amené à revêtir.',
                    opinion: 'Très beaux textes.  Début très prenant mais l\'histoire devient moins captivante au fil de la lecture.  Ce roman reste toutefois un grand classique très intéressant et, sans conteste, à lire.'
                },
                {
                    id: 'clMalrauxCH',
                    title: 'la condition humaine',
                    author: 'Malraux',
                    edition: 'folio',
                    summary: 'Pas encore de résumé ...',
                    opinion: 'Pas encore d\'opinion.' 
                }
                ]
            }
        },
    }
</script>