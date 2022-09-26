<template>
    <base-card>
        <!-- le @click est automatiquement appliqué au <button> du BaseButton car c'est l'élément html 'root' -->
        <base-button @click="setSelectedBtn('stored-resources')">Livres lus</base-button>
        <base-button @click="setSelectedBtn('add-book')">Ajouter un livre</base-button>
    </base-card>
    <component :is="selectedBtn"></component>
</template>

<script>
    import StoredResources from './StoredResources.vue';
    import AddBook from './AddBook.vue';

    export default {
        components: {
            StoredResources,
            AddBook
        },

        data(){
            return{
                selectedBtn: 'stored-resources',

            storedBooks: [
                {
                    id: 'clStendhalRN',
                    title: 'Le rouge et le noir',
                    author: 'Stendhal',
                    edition: 'Les Cent Chefs-d\'oeuvre',
                    summary: 'Julien Sorel, fils de charpentier, doté de capacités intellectuelles supérieures, tente de s\'élever dans la société. Passionné par Napoléon, il rêve d\'une grande destinée en revêtant l\'habit de soldat (rouge) mais c\'est celui du clergé (noir) qui lui sera réservé.',
                    opinion: 'Très beaux textes.  Début très prenant mais l\'histoire devient moins captivante au fil de la lecture.  Ce roman reste toutefois un grand classique très intéressant et, sans conteste, à lire.',
                    link: 'https://awebstyle.be'
                },
                {
                    id: 'clMalrauxCH',
                    title: 'La condition humaine',
                    author: 'Malraux',
                    edition: 'folio',
                    summary: 'Pas encore de résumé ...',
                    opinion: 'Pas encore d\'opinion.',
                    link: 'https://awebstyle.be' 
                }
                ]

            } 
        },

        provide(){
            return {
                resources: this.storedBooks
            };
        },

        methods: {
            setSelectedBtn(btn){
                this.selectedBtn = btn;
            }
        }
    }
</script>