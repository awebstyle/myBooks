<template>
    <header>
        <h1>{{ title }}</h1>
    </header>
</template>

<script>
    export default {
        props: ['title']
    }
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Kalam:wght@700&display=swap');

    header {
    width: 100%;
    height: 5rem;
    background-color: #154553;
    display: flex;
    justify-content: center;
    align-items: center;
    }

    header h1 {
    color: white;
    margin: 0;
    font-family: 'Kalam', cursive;
    }
    
   
    
</style>