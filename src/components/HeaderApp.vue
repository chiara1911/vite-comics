<template>
    <header>
  <div class="container mt-1">  
   <div class="d-flex justify-content-between">       
            <img src="../assets/images/dc-logo.png" alt="">        
        
            <ul class="d-flex flex-row justify-content-between align-items-center">
                <li v-for ="navLink in navLinks" class="p-1 text-uppercase"><a href="#">{{navLink}}</a></li>
            </ul>
       
    </div>
    </div>
</header>
</template>

<script>
    export default {
        name: 'HeaderApp',

        data(){
            return {
                navLinks :[               
                'characters',
                'comics',
                'movies',
                'tv',
                'games',
                'collectibles',
                'videos',
                'fans',
                'news',
                'shop'
                ],
            }
        }
    } 

    
</script>

<style lang="scss" >

    li{
        list-style: none;
    }

</style>