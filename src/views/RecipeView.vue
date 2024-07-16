<template>
    <div class="recipe">
        <h1 class="title">Pizza</h1>
        <div class="recipe__info">
            <img class="img" src="/src/assets/default.jpg"/>
            <div class="ingredients__wrapper">
                <h3>Ingredients</h3>
                <ul class="ingredients">
                    <li class="ingredient"><p>cheese</p> <p>2 slices</p></li>
                    <li class="ingredient"><p>cheese ham</p> <p>2 slices</p></li>
                    <li class="ingredient"><p>mushrooms</p> <p>10</p></li>
                    <li class="ingredient"><p>water</p> <p>1 cup</p></li>
                    <li class="ingredient"><p>oregano</p> <p>1 pinch</p></li>
                </ul>
            </div>
        </div>
        <h3>Instructions</h3>
        <div class="instructions__wrapper">
            <div>
                <h4>Step 1</h4>
                <img class="instruction__img" src="/src/assets/default.jpg"/>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos dolores iure ducimus labore! Ratione, sit accusamus quia animi, labore dolore eligendi, quod quasi est delectus modi odio ullam laborum mollitia.
                Eligendi ex deserunt, debitis nemo soluta esse molestias, quasi accusantium eius cum vitae repellat recusandae pariatur placeat quos. Porro ipsum saepe consectetur voluptates culpa quas perspiciatis doloremque soluta recusandae magni?
                </p>
            </div>
            <div>
                <h4>Step 1</h4>
                <img class="instruction__img" src="/src/assets/default.jpg"/>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos dolores iure ducimus labore! Ratione, sit accusamus quia animi, labore dolore eligendi, quod quasi est delectus modi odio ullam laborum mollitia.
                Eligendi ex deserunt, debitis nemo soluta esse molestias, quasi accusantium eius cum vitae repellat recusandae pariatur placeat quos. Porro ipsum saepe consectetur voluptates culpa quas perspiciatis doloremque soluta recusandae magni?
                </p>
            </div>
            <div>
                <h4>Step 1</h4>
                <img class="instruction__img" src="/src/assets/default.jpg"/>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos dolores iure ducimus labore! Ratione, sit accusamus quia animi, labore dolore eligendi, quod quasi est delectus modi odio ullam laborum mollitia.
                Eligendi ex deserunt, debitis nemo soluta esse molestias, quasi accusantium eius cum vitae repellat recusandae pariatur placeat quos. Porro ipsum saepe consectetur voluptates culpa quas perspiciatis doloremque soluta recusandae magni?
                </p>
            </div>
            <div>
                <h4>Step 1</h4>
                <img class="instruction__img" src="/src/assets/default.jpg"/>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos dolores iure ducimus labore! Ratione, sit accusamus quia animi, labore dolore eligendi, quod quasi est delectus modi odio ullam laborum mollitia.
                Eligendi ex deserunt, debitis nemo soluta esse molestias, quasi accusantium eius cum vitae repellat recusandae pariatur placeat quos. Porro ipsum saepe consectetur voluptates culpa quas perspiciatis doloremque soluta recusandae magni?
                </p>
            </div>
            <div>
                <h4>Step 1</h4>
                <img class="instruction__img" src="/src/assets/default.jpg"/>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Eos dolores iure ducimus labore! Ratione, sit accusamus quia animi, labore dolore eligendi, quod quasi est delectus modi odio ullam laborum mollitia.
                Eligendi ex deserunt, debitis nemo soluta esse molestias, quasi accusantium eius cum vitae repellat recusandae pariatur placeat quos. Porro ipsum saepe consectetur voluptates culpa quas perspiciatis doloremque soluta recusandae magni?
                </p>
            </div>
            
        </div>
    </div>
</template>

<style scoped>

.recipe{
    padding: 0 1em;
}

.img{
    width: 100%;
    border-radius: .5rem;
    aspect-ratio: 16/9;
    object-fit: cover;
}

.ingredient{
    display: flex;
    gap: 1rem;
    border-bottom: solid 1px var(--color-primary)
}

.ingredient > p{
    width: 50%;
}

.instruction__img{
    width: 100%;
    border-radius: .5rem;
    aspect-ratio: 16/9;
    object-fit: cover;
}

@media (min-width: 800px) {
    .img{
        max-width: 50%;
    }

    .recipe__info{
        display: flex;
        justify-content: end;
    }

    .ingredients__wrapper{
        padding-left: 1em;
        width: 100%;
    }

    .instructions__wrapper{
        display: grid;
        grid-template-columns: auto auto;
        gap: 1rem;
        
    }
}



</style>