<template>
    <h1>Dernières lectures</h1>
    <ul>
      <book-resource v-for="book in storedBooks" :key="book.id"
        :title="book.title"
        :author="book.author"
        :edition="book.edition"
        :summary="book.summary"
        :opinion="book.opinion"
        :link="book.link"
      >
      </book-resource>  
    </ul>
</template>

<script>
    import BookResource from './components/books/BookResource.vue';
    export default {
        components: {
            BookResource
        },
        data(){
            return {
                storedBooks: [
                {
                    id: 'clStendhalRN',
                    title: 'le rouge et le noir',
                    author: 'Stendhal',
                    edition: 'Les Cent Chefs-d\'oeuvre',
                    summary: 'Julien Sorel, fils de charpentier, doté de capacités intellectuelles supérieurs, tente de s\'élever dans la société. Passionné par Napoléon, il rêve d\'une grande destinée en revêtant l\'habit de soldat (rouge) mais c\'est celui du clergé (noir) qu\'il sera amené à revêtir.',
                    opinion: 'Très beaux textes.  Début très prenant mais l\'histoire devient moins captivante au fil de la lecture.  Ce roman reste toutefois un grand classique très intéressant et, sans conteste, à lire.',
                    link: 'https://awebstyle.be'
                },
                {
                    id: 'clMalrauxCH',
                    title: 'la condition humaine',
                    author: 'Malraux',
                    edition: 'folio',
                    summary: 'Pas encore de résumé ...',
                    opinion: 'Pas encore d\'opinion.',
                    link: 'https://awebstyle.be' 
                }
                ]
            }
        },
    }
</script>