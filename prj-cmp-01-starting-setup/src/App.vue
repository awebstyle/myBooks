<template>
    <TheHeader title="Mes dernières lectures"/>
    <the-resources></the-resources>
</template>

<script>
    
    import TheHeader from './components/layout/TheHeader.vue';
    import TheResources from './components/books/TheResources.vue';

    export default {
        components: {
            TheHeader,
            TheResources
        },
        data(){
            return {
                
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
  background-repeat: no-repeat;
}

h1 {
  text-align: center ;
}
</style>