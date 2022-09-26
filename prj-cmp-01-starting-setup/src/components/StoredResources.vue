<template>
    <ul>
      <book-resource v-for="book in resources" :key="book.id"
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
    import BookResource from './books/BookResource.vue'
    export default{
        components: {
            BookResource
        },
        props: ['resources']
    }
</script>

<style scoped>
    ul {
        list-style: none;
        margin: 0;
        padding: 0;
        margin: auto;
        max-width: 40rem;
    }
</style>