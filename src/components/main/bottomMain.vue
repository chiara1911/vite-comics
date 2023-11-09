<template>
    <div id="bottom-main" >
    <div class="container">
    <ul class="d-flex flex-row justify-content-between m-0 p-2">
                <li v-for ="el in items" class="p-1 text-light text-uppercase d-flex flex-row">
                    <a href="#"><img :src="el.img" :alt="el.text" class=""></a>
                    <span class="p-2 d-flex flex-wrap align-content-center ">{{el.text}}</span></li>
    </ul>
</div>
</div>
</template>

<script>
    export default {
        name:'bottomMain',
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

<style lang="scss" scoped>

</style>