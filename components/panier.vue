<template>
    <div class="panier" id="panier">
        <div class="top" id="panierTop">
            <p>Votre panier</p>
            <span class="material-symbols-outlined" @click="$emit('closePanier')">
                close
            </span>
        </div>
        <br>
        <div class="center" id="panierCenter">
            <div class="tonal">
                <span class="material-symbols-outlined">
                    shopping_basket
                </span>
            </div>
            <p>Panier vide .</p>

            <br> <br> <br> <br>
            <div class="box">
                <p>Samsung</p>
            </div>
            <div class="box">
                <p>Iphone</p>
            </div>
            <div class="box">
                <p>Ordinateur</p>
            </div>
            <br> <br>
            <div class="home">
                <p>Retour a l'accueil</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'panier',

}
</script>

<style scoped>
.panier {
    height: 100vh;
    position: fixed;
    right: 0;
    top: 0;
    background-color: white;
    z-index: 100;
    color: black;
    /* padding: 5px 20px 5px 20px; */
    width: 0%;
    transition: 0.3s ease;

}

.panier .top {
    display: none;
    justify-content: space-between;
    align-items: center;
    font-size: 1.5rem;
    font-weight: 700;
}

.panier .center {
    display: none;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.center .tonal {
    background-color: rgba(128, 128, 128, 0.152);
    padding: 15px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
}

.center .box {
    width: 100%;
    border: 1px solid rgba(128, 128, 128, 0.559);
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
}

.center .home {
    width: 100%;
    border-radius: 9999px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
    background-color: orangered;
    color: white;
    font-weight: 600;
}</style>