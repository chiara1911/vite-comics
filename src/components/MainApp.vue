<template>
    <div class="container">
<div id="top-main" class="bg-dark">
    <h2 class="text-light py-5"> -- > Content Goes here  -- </h2>
</div>
<div id="bottom-main">
    <ul class="d-flex flex-row justify-content-between ">
                <li v-for ="(el,index) in items" class="p-3 ">
                    <img :src="el.img" alt="">
                    <span>{{el.text}}</span></li>
    </ul>
</div>
    
    <div class="p-5">
        
    </div>
</div>
</template>

<script>
    export default {
        name: 'MainApp',
        data(){
            return {
                items:[
                    {
                        img: "/src/assets/images/buy-comics-digital-comics.png",
                        text: "DIGITAL COMICS"
                    },
                    {
                        img: "/src/assets/images/buy-comics-merchandise.png",
                        text: "dc merchandise"
                    },
                    {
                        img: "/src/assets/images/buy-comics-subscriptions.png",
                        text: "subcription"
                    },
                    {
                        img: "/src/assets/images/buy-comics-shop-locator.png",
                        text: "comic shop locator"
                    },

                ]
            }
        }
   

    
    }
    </script>

<style lang="scss">
    #top-main{
    background-color: black;
   }
    #bottom-main{
    background-color: blue;
   }

</style>