<script setup>
import RecipeCard from '../components/recipe/RecipeCard.vue';
</script>
<template>
    <ul class="recipes__list">
       <RecipeCard v-for="index in 20"/>
     </ul>
</template>

<style scoped>

.recipes__list{
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 1rem;
    padding: 0 1em;
}


@media (min-width: 600px) {
    .recipes__list{
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: center;
    }

    .recipe{
        max-width: 30%;
    }
}
</style>