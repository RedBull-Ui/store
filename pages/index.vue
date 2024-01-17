<template>
  <div class="body">
    <div class="top">
      <appNav />
      <p>Never <br> stop <br> exploring</p> <br>
      <h3>Get your gear today</h3> <br> <br> <br>
      <button><span>Shop Hiking GEAR</span> <span>--></span></button>
    </div>
  </div>
  
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700;900&display=swap');

*,::after, ::before{
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  box-sizing: border-box;

}
.body{
  width: 100%;
}

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
</style>

<script>
import appNav from '/components/appNav.vue'
export default {
  components: {
    appNav
  },
  name: 'IndexPage'
}
</script>