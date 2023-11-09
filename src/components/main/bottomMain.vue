<template>
    <div id="bottom-main" >
    <div class="container">
    <ul class="d-flex flex-row justify-content-between m-0">
                <li v-for ="el in items" class="p-3 text-light text-uppercase">
                    <a href="#"><img :src="el.img" :alt="el.text" class="px-2 w-25 h-50 "></a>
                    <span>{{el.text}}</span></li>
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