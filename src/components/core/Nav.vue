<script setup>
import MenuIcon from '../icons/MenuIcon.vue';
import CloseIcon from '../icons/CloseIcon.vue';
import { ref} from 'vue';

const showMobileNav = ref(false);

const showMenu = () => {
    showMobileNav.value = true;
};

const hideMenu = () => {
    showMobileNav.value = false;
};

</script>

<template>
    <nav class="nav">
        <p class="logo">Logo</p>
        <ul class="nav__list">
            <li class="hideOnMobile">
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li class="hideOnMobile">
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li class="hideOnMobile"> 
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li class="hideOnMobile">
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li class="nav__icon showOnMobile">
                <MenuIcon @click="showMenu()"/>
            </li>
        </ul>
        <ul class="nav__list--mobile" ref="nav" v-if="showMobileNav">
            <li class="close">
                <CloseIcon @click="hideMenu()"/>
            </li>
            <li>
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li>
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li>
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
            <li>
                <RouterLink class="link" :to="{name: 'recipes'}">
                    Recipes
                </RouterLink>
            </li>
        </ul>
    </nav>
</template>

<style scoped>
    .nav{
        padding: 1em;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: white;
    }

    .nav__list{
        display: flex;
        justify-content: space-between;
        margin: 0;
        align-items: center;
        gap: 2rem;
    }

    .nav__list li{
        width: 100%;
    }

    .nav__list--mobile{
        position: absolute;
        gap: 1rem;
        top: 0;
        left: 0;
        width: 100%;
        background-color: white;
        height: 100vh;
        padding: 0 2rem;
    }

    .nav__list--mobile li{
        padding: 1em 0;
    }

    .nav__icon{
        display: none;
    }
    .logo{
        margin: 0;
    }

    .close{
        display: flex;
        justify-content: end;
    }   

    .link{
        text-decoration: none;
        color: black;
    }

    @media (max-width: 800px) {
        .hideOnMobile{
            display: none;
        }

        .showOnMobile{
            display: inline-block;
        }
    }
</style>