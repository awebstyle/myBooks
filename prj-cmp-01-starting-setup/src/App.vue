<template>
    <TheHeader title="Mes dernières lectures"/>
    <stored-resources
        :resources="storedBooks"
    >
    </stored-resources>
</template>

<script>
    import StoredResources from './components/StoredResources.vue';
    import TheHeader from './components/layout/TheHeader.vue';

    export default {
        components: {
            StoredResources,
            TheHeader
        },
        data(){
            return {
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
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=League+Spartan:wght@200;300&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'League Spartan', sans-serif;
}

body {
  margin: 0;
  background-image: url('./img/book.jpg');
  background-size: cover;
}

h1 {
  text-align: center ;
}
</style>