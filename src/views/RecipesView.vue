<template>
    <div class="container">
        <nav class="nav">
        <h3 class="logo">Logo</h3>
        <ul class="nav__list">
            <li class="link">
                <RouterLink :to="{name: 'recipes'}" class="link">
                    Recipes
                </RouterLink>
            </li>
            <li class="link">
                <RouterLink :to="{name: 'recipes'}" class="link">
                    Favorite
                </RouterLink>
            </li>
            <li class="link">
                <RouterLink :to="{name: 'recipes'}" class="link">
                    Settings
                </RouterLink>
            </li>
        </ul>
        </nav>
        <div class="container__content">
            <form class="search">
                <input class="search__input">
                <button class="search__submit">search</button>
            </form>
            <h3>Recipes (26)</h3>
            <ul class="recipes__list">
                <li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
                </li><li class="recipes__item">
                    Pizza
                </li><li class="recipes__item">
                    Pizza
                </li><li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
                </li>
                <li class="recipes__item">
                    Pizza
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
</template>