<script setup>
import ClockIcon from '../components/icons/ClockIcon.vue';
import CartIcon from '../components/icons/CartIcon.vue';
import PersonIcon from '../components/icons/PersonIcon.vue';
import SearchIcon from '../components/icons/SearchIcon.vue';
</script>
<template>
    <div class="container">
        <div class="container__content">
            <div>
                <form class="search">
                <input class="search__input">
                <button class="search__submit"><SearchIcon/></button>
                </form>
            <ul class="recipes__list">
                <li v-for="i in 20">
                    <div class="recipe">
                        <img class="recipe__img" src="../assets/default.jpg"/>
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
            </ul>
            <div class="pagination"> 
                <button>< Back</button>
                <input value="1">
                <div> / </div>
                <div>10</div>
                <button>Next ></button>
            </div>
        </div>
        </div>
    </div>
</template>