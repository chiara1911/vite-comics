<template>
    
   <main>
<div id="top-main" class="bg-dark">
    <div class="container">
    <h2 class="text-light py-5"> -- > Content Goes here  -- </h2>
</div>
<bottomMain />
</div>
</main>

</template>

<script>
import bottomMain from './main/bottomMain.vue';
    export default {
        name: 'MainApp',
        components: {
            bottomMain
        }
       
   

    
    }
    </script>

<style lang="scss">
    #top-main{
    background-color: black;
   }
    #bottom-main{
    background-color: rgb(0, 115, 255);
   }

</style>