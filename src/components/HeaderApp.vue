<template>
  <div class="container mt-5">  
   <div class="d-flex justify-content-between">
        <div>
            <img src="../assets/images/dc-logo.png" alt="">
        </div>
        <div>
            <ul class="d-flex flex-row justify-content-between ">
                <li v-for ="navLink in navLinks" class="p-3 ">{{ navLink}}</li>
            </ul>
        </div>
    </div>
    </div>
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