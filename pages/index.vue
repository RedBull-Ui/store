<template>
  <div class="body">
    <div class="top">
      <appMenu />
      <appNav v-on:menu="menuTogle" />
      <br> <br> <br>
      <p>Never <br> stop <br> exploring</p> <br>
      <h3>Get your gear today</h3> <br> <br> <br>
      <button>
        <span>Shop Hiking GEAR</span> <span>--></span>
      </button>
    </div>
    <br> <br>
    <!-- slider jour  -->
    <topJour />
    <!-- slider jour  -->

    <div class="center">
      <h1>Meilleure <br> des ventes</h1> <br> <br> <br> <br>
      <button><span>Visiter maintenant</span> <span>--></span></button>
    </div>

    <!-- categories -->
    <categoriesIndex />
    <!-- categories -->

    <!-- les sold  -->
    <soldeIndex />
    <!-- les sold  -->
  </div>
</template>

<script>
import appMenu from '~/components/appMenu.vue'
import appNav from '~/components/appNav.vue'
import topJour from '~/components/topJour.vue'
import categoriesIndex from '~/components/categoriesIndex.vue'
import soldeIndex from '~/components/soldeIndex.vue'

export default {
  components: {
    appNav,
    topJour,
    categoriesIndex,
    soldeIndex,
    appMenu
  },
  methods: {
    menuTogle() {
      var menu = document.getElementById('menu');

      menu.style.width = '100%'

     document.body.style.overflow ='hidden';


      var elementsTonal = document.querySelectorAll('.tonalMenu');

     // Sélectionnez tous les éléments avec la classe "tonal" et le h1
      var elementsTonalAndH1 = document.querySelectorAll('.tonalMenu, h1');

      // Parcourez chaque élément
      elementsTonalAndH1.forEach(function (element) {
        // Modifiez la propriété CSS 'display' à 'block'
        element.style.display = 'flex';
      });

    }
  },
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700;900&display=swap');

*,::after, ::before{
  margin: 0 ;
  padding: 0 ;
  font-family: 'Poppins', sans-serif;
  box-sizing: border-box;

}

.body {
  width: 100% ;
  margin: 0px ;
  background-color: rgba(227, 228, 230, 0.363);
}

/* menu  */


/* menu  */
.top{
  height: 75vh;
  background: url(/accueil.jpg) center/cover;
  color: white;
  width: 100%;
  display: flex;
  padding: 5px;
  flex-direction: column;

}
.top p{
  text-align: right;
  font-size: 3rem;
  font-weight: bolder;
}
.top h3{
  text-align: right;
}
.top button{
  width: 300px;
  background-color: orangered;
  color: white;
  border: none;
  border-radius: 9999px;
  height: 50px;
  margin-left: auto;
  margin-right: auto;
  font-weight: 900;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
}

/* center  */
.center {
  padding: 20px;
  height: 580px;
  background: url(/tecnologie.jpg) center/cover;
}
.center h1{
  color: white;
  font-size: 3rem;
}
.center button{
  margin-top: 150px;
  width: 300px;
  background-color: orangered;
  color: white;
  border: none;
  border-radius: 9999px;
  height: 50px;
  margin-left: auto;
  margin-right: auto;
  font-weight: 900;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
}
/* center  */

/* categories  */
.categories{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
/* categories  */

</style>

