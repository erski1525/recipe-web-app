<script setup>
import ClockIcon from '../icons/ClockIcon.vue';
import CartIcon from '../icons/CartIcon.vue';
import PersonIcon from '../icons/PersonIcon.vue';
import { useRouter } from 'vue-router';

const router = useRouter();

</script>

<template>
<li class="recipe" @click="router.push({name: 'recipe', params: {id: 0}})">
    <div class="overlay">
        <img class="recipe__img" src="/src/assets/default.jpg"/>
    </div>
    <div class="recipe__info">
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

.recipe__img{
    width: 100%;
    object-fit: cover;
    margin:0;
    padding: 0;
    vertical-align: top;

}

.recipe__info{
    border-left: solid 2px white;
    border-bottom: solid 2px white;
    border-right: solid 2px white;
    border-radius: 0 0 .5rem .5rem;
    padding-top: 1em;
}

.recipe__title{
    text-align: center;
    padding-bottom: 1rem;
    margin: 0;
    border-bottom: 2px solid var(--color-primary);
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
    color: var(--color-primary)
}

.overlay{
    position: relative;
}

.recipe:hover{
    cursor: pointer;
}
.recipe:hover .overlay::after{
    content: '\A';
    position: absolute;
    width: 100%; height:100%;
    top:0; left:0;
    background:rgba(0,0,0,0.5);
}

.recipe:hover .recipe__info {
    border-left: solid 2px var(--color-primary);
    border-bottom: solid 2px var(--color-primary);
    border-right: solid 2px var(--color-primary);
}

</style>