<template>
   <h2>header</h2>

   <ul class="d-flex flex-row flex-nowrap">
    <li v-for ="navLink in navLinks">{{ navLink}}</li>
   </ul>
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

<style lang="scss" scoped>

</style>