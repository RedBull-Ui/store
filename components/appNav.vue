<template>
    <div class="nav">
        <h1>LOGO</h1>
        <div class="tonal">
            <span class="material-symbols-outlined">
                search
            </span>
        </div>
        <div class="tonal">
            <span class="material-symbols-outlined">
                shopping_basket
            </span>
        </div>
        <div class="tonal">
            <span class="material-symbols-outlined">
                menu
            </span>
        </div>
    </div>
</template>

<style scoped>
.nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;
}
h1{
    margin-right: 40px;
}
.material-symbols-outlined {
    font-size: 1.8rem;
}
.tonal{
    background-color: white;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    color: orangered;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>

