<template>
    <div class="menu" id="menu">
        <div class="menu-nav">
            <h1>LOGO</h1>

            <div class="tonal">
                <span class="material-symbols-outlined">
                    shopping_basket
                </span>
            </div>
            <div class="tonal">
                <span class="material-symbols-outlined" >
                    close
                </span>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
.menu {
    position: absolute;
    z-index: 100;
    right: 0;
    top: 0;
    width: 0%;
    height: 100vh;
    background-color: #232323;
}

.menu-nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;
}

h1 {
    margin-right: 40px;
    display: none;
}

.material-symbols-outlined {
    font-size: 1.8rem;
}

.tonal {
    background-color: white;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    color: orangered;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;

    display: none;
}
</style>
