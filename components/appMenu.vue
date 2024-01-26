<template>
    <div class="menu" id="menu">
        <div class="menu-nav">
            <h1 id="h1Menu">LOGO</h1>

            <div class="tonalMenu">
                <span class="material-symbols-outlined">
                    shopping_basket
                </span>
            </div>
            <div class="tonalMenu" >
                <span class="material-symbols-outlined" @click="menuClose()">
                    close
                </span>
            </div>
        </div>
        <div class="menuItem" @click="$emit('telephone')">
            <p>Telephone</p>
            <span class="material-symbols-outlined">
                chevron_right
            </span>
        </div>
        <div class="menuItem">
            <p>Ordinateur</p>
            <span class="material-symbols-outlined">
                chevron_right
            </span>
        </div>
        <div class="menuItem">
            <p>Frigo</p>
            <span class="material-symbols-outlined">
                chevron_right
            </span>
        </div>
        <div class="menuItem">
            <p>Tablette</p>
            <span class="material-symbols-outlined">
                chevron_right
            </span>
        </div>
        <div class="menuItem">
            <p>Accessoires</p>
            <span class="material-symbols-outlined">
                chevron_right
            </span>
        </div>

        <h4>Powered by Privat's Labs</h4>

    </div>
</template>


<style scoped>
.menu {
    display: flex;
    flex-direction: column;
    position: fixed;
    z-index: 100;
    right: 0;
    top: 0;
    width: 0%;
    max-height: 100%;
    min-height: 100%;
    background-color: #232323;
    transition: 0.2s ease-in-out;
    overflow: hidden;
}

.menu-nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    color: white;
}

#h1Menu {
    margin-right: 40px;
    display: none;
}

.material-symbols-outlined {
    font-size: 1.8rem;
}

.tonalMenu {
    background-color: white;
    border-radius: 50%;
    width: 50px;
    height: 50px;
    color: orangered;
    align-items: center;
    justify-content: center;
    cursor: pointer;

    display: none;
}

/* les menu itels ici  */

.menuItem {
    padding: 0 20px 0px 20px;
    font-weight: 700;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
}
span{
    color: orangered;
}

/* les menu itels ici  */

h4{
    position: fixed;
    bottom: 0;
    margin-left: 24.5%;
    font-family: Arial, Helvetica, sans-serif;
}
</style>


<script>
export default {
    methods: {
        menuClose() {
            var menu = document.getElementById('menu');

            menu.style.width = '0%'
            document.body.style.overflow = 'scroll';


            var elementsTonal = document.querySelectorAll('.tonal');

            // Sélectionnez tous les éléments avec la classe "tonal" et le h1
            var elementsTonalAndH1 = document.querySelectorAll('.tonalMenu, #h1Menu');

            // Parcourez chaque élément
            elementsTonalAndH1.forEach(function (element) {
                // Modifiez la propriété CSS 'display' à 'block'
                element.style.display = 'none';
            });

        }
    },
}
</script>
