<template>
    <button :type="type" :class="mode">
        <slot></slot>
    </button>
</template>

<script>
    export default {
        props: ['type', 'mode']
    }
</script>

<style scoped>
    button{
        background: #875552;
        color: #fff;
        border-radius: 3px;
        padding: .5rem 1.5rem;
        cursor: pointer;
    }

    button:hover,
    button:active {
        background-color: #154553;
        border-color: #154553;
    }

    .flat {
        background-color: transparent;
        color: #875552;
        border: none;
        }

    .flat:hover,
    .flat:active {
    background-color: #875552;
    color: #fff;
}
</style>