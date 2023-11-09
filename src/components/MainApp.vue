<template>
    
   
<div id="top-main" class="bg-dark">
    <div class="container">
    <h2 class="text-light py-5"> -- > Content Goes here  -- </h2>
</div>
<div id="bottom-main">
    <ul class="d-flex flex-row justify-content-between ">
                <li v-for ="el in items" class="p-3 text-light text-uppercase">
                    <a href=""><img :src="el.img" :alt="el.text" class="px-2 w-25 h-75 "></a>
                    <span>{{el.text}}</span></li>
    </ul>
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
                    {
                        img: "/src/assets/images/buy-dc-power-visa.svg",
                        text: "dc power visa"
                    }

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
    background-color: rgb(0, 115, 255);
   }

</style>