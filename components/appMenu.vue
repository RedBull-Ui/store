<template>
    <div class="menu" id="menu">
        <div class="menu-nav">
            <h1 id="h1Menu">LOGO</h1>

            <div class="tonalMenu">
                <span class="material-symbols-outlined">
                    shopping_basket
                </span>
            </div>
            <div class="tonalMenu" @click="menuClose()">
                <span class="material-symbols-outlined" >
                    close
                </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
      methods: {
        menuClose() {
            var menu = document.getElementById('menu');

            menu.style.width = '0%'

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

<style scoped>
.menu {
    position: absolute;
    z-index: 100;
    right: 0;
    top: 0;
    width: 0%;
    height: 100vh;
    background-color: #232323;
    transition: 0.2s ease-in-out;
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
</style>
