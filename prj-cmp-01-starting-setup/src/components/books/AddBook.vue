<template>
    <base-card id="bookAdd">
        <form>
            <div class="form-control">
                <label for="title">Titre</label>
                <input type="text" id="title" name="title">
            </div>
            <div class="form-control">
                <label for="author">Auteur</label>
                <input type="text" id="author" name="author">
            </div>
            <div class="form-control">
                <label for="edition">Édition</label>
                <input type="text" id="edition" name="edition">
            </div>
            <div class="form-control">
                <label for="summary">Résumé</label>
                <textarea id="summary" name="summary" rows="3"></textarea>
            </div>
            <div class="form-control">
                <label for="opinion">Avis</label>
                <textarea id="opinion" name="opinion" rows="3"></textarea>
            </div>
            <div class="form-control">
                <label for="link">Lien vers le résumé en images</label>
                <input type="url" id="link" name="link">
            </div>
            <div>
                <base-button type="submit">Ajouter le livre</base-button>
            </div>
        </form>
    </base-card>
</template>

<style scoped>
    label {
    font-weight: bold;
    display: block;
    margin-bottom: 0.5rem;
    }

    input,
    textarea {
    display: block;
    width: 100%;
    font: inherit;
    padding: 0.15rem;
    border: 1px solid #ccc;
    }

    input:focus,
    textarea:focus {
    outline: none;
    border-color: #3a0061;
    background-color: #cdd4d2;
    }

    .form-control {
    margin: 1rem 0;
    }

    
</style>