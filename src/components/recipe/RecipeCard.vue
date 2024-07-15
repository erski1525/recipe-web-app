<script setup>
import ClockIcon from '../icons/ClockIcon.vue';
import CartIcon from '../icons/CartIcon.vue';
import PersonIcon from '../icons/PersonIcon.vue';
</script>
<template>
    <li class="recipe">
        <img class="recipe__img" src="/src/assets/default.jpg"/>
        <p class="recipe__title">Pizza</p>
        <div class="recipe__description">
            <div class="icon__wrapper">
                <ClockIcon/>
                20min
            </div>
            <div class="icon__wrapper">
                <CartIcon/>
                12,99 zł
            </div>
            <div class="icon__wrapper">
                <PersonIcon/>
                2 osoby
            </div>
        </div>
    </li>
</template>

<style scoped>

.recipe{
    background-color: #FFF;
    border-radius: .5rem;
    overflow: hidden;
    max-width: 600px;
}

.recipe:hover{
    cursor: pointer;
}

.recipe__img{
    margin-bottom: 1rem;
    width: 100%;
    object-fit: cover;
}

.recipe__title{
    margin-top: 0;
    text-align: center;
    padding-bottom: 1em;
    border-bottom: 1px solid var(--color-primary);
}

.recipe__description{
    padding: 1em;
    display: flex;
    justify-content: space-around;
}

.icon__wrapper{
    display: flex;
    flex-direction: column;
    gap: 1rem;
    align-items: center;
}

@media (min-width: 600px) {
    .recipe{
        max-width: 30%;
    }
}
</style>