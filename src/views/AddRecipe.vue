<script setup>
import CloseIcon from '../components/icons/CloseIcon.vue';
</script>
<template>
    <div class="container">
        <h1>Add recipe</h1>
        <form>
            <div class="input__group">
                <label>Title</label>
                <input class="input" placeholder="Pizza" type="text"/>
            </div>
            <div class="input__group">
                <label>Image (optional)</label>
                <img class="img" src="/src/assets/default.jpg"/>
                <input type="file"/>
            </div>
            <div class="input__group">
                <h4>Ingredients</h4>
                <ul>
                    <li class="ingredient">
                        <p>cheese</p>
                        <p>2 slices</p>
                        <CloseIcon/>
                    </li>
                    <li class="ingredient">
                        <p>ham</p>
                        <p>2 slices</p>
                        <CloseIcon/>
                    </li>
                    <li class="ingredient">
                        <p>mushrooms</p>
                        <p>10 units</p>
                        <CloseIcon/>
                    </li>
                </ul>
                <div class="input__group--row">
                    <div class="input__group grow">
                        <label>Name</label>
                        <input type="text" class="input--row left" placeholder="Cheese"/>
                    </div>
                    <div class="input__group grow">
                        <label>Amount</label>
                        <input type="text" class="input--row right" placeholder="2 slices"/>
                    </div>
                </div>
                <button class="submit">Add ingredient</button>
            </div>
            <div class="input__group">
                <h4>Instructions</h4>
                <ul>
                    <li class="instruction">
                        <div class="instruction__action"><p>Step 1</p><CloseIcon/></div>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repudiandae ex deleniti, blanditiis laudantium amet enim cumque, dicta reiciendis voluptates itaque officiis eum nobis repellat possimus quaerat obcaecati est eligendi asperiores.
                        Qui suscipit unde iste saepe asperiores consectetur ad laborum cumque non ducimus perspiciatis magnam quos sint assumenda similique vitae facere, itaque voluptatibus quod commodi quaerat necessitatibus. Neque cum totam ex.
                    </li>
                    <li class="instruction">
                        <div class="instruction__action"><p>Step 2</p><CloseIcon/></div>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repudiandae ex deleniti, blanditiis laudantium amet enim cumque, dicta reiciendis voluptates itaque officiis eum nobis repellat possimus quaerat obcaecati est eligendi asperiores.
                        Qui suscipit unde iste saepe asperiores consectetur ad laborum cumque non ducimus perspiciatis magnam quos sint assumenda similique vitae facere, itaque voluptatibus quod commodi quaerat necessitatibus. Neque cum totam ex.
                    </li>
                    <li class="instruction">
                        <div class="instruction__action"><p>Step 3</p><CloseIcon/></div>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repudiandae ex deleniti, blanditiis laudantium amet enim cumque, dicta reiciendis voluptates itaque officiis eum nobis repellat possimus quaerat obcaecati est eligendi asperiores.
                        Qui suscipit unde iste saepe asperiores consectetur ad laborum cumque non ducimus perspiciatis magnam quos sint assumenda similique vitae facere, itaque voluptatibus quod commodi quaerat necessitatibus. Neque cum totam ex.
                    </li>
                </ul>
                <textarea class="input" placeholder="Pizza" type="text" rows="5"></textarea>
                <button class="submit">Add instruction</button>
            </div>
            <div class="form__actions">
                <button class="submit">Create recipe</button>
                <button class="submit">Cancel</button>
            </div>
        </form>
    </div>
</template>

<style scoped>
.container{
    padding: 0 1em;
}

.img{
    border-radius: .5rem;
}

.input{
    width: 100%;
    padding: 1em;
    border-radius: .5rem;
    border: none;
}

.input__group{
    margin-top: 1rem;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

.ingredient{
    display: flex;
    border-bottom: 1px solid var(--color-primary);
    align-items: center
}

.ingredient > p{
    width: 50%;
}

.input__group--row{
    display: flex;
}

.submit__wrapper{
    display: flex;
    align-items: end;
}

.grow{
    flex: 1;
}

.input--row{
    padding: 1em;
    border: none;
}

.left{
    padding: 1em;
    border-radius: .5rem 0 0 .5rem;
    border: none;
}

.right{
    padding: 1em;
    border-radius: 0 .5rem .5rem 0;
    border: none;
}

.submit{
    padding: 1em;
    border: none;
}

.instruction{
    border-bottom: 1px solid var(--color-primary);
    padding: 1em 0;
}

.instruction__action{
    display: flex;
    justify-content: space-between;
}

.form__actions{
    display: flex;
    margin-top: 2rem;
}

.form__actions button{
    flex: 1;
}
</style>