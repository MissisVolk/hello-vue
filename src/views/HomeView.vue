<template>
  <!-- <div class="home">
    <img alt="Vue logo" src="../assets/image-menu/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div> -->
  <h2> Добро пожаловать!</h2>
  <a href="#" class="btn btn-succes"> Add product</a>
  <div> Мы любим туризм, альпинизм и своё дело! Добро пожаловать в наш магазин!
    <div>
      <img src="./MyCollages.jpg" alt="MyCollagesSS">
    </div>
  </div>
  <MyDialog></MyDialog>
</template>



<script>
export default {
  name: "HomeView",
}

// // @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// import MyDialog from '@/components/ui/ui/elements/MyDialog.vue';

// export default {
//   name: 'HomeView',
//   components: {
//     HelloWorld,
//     MyDialog
// }
// }
</script>

<style scoped>

</style>