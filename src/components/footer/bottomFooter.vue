<template>
   
    <div id="bottomFooter" >
        <div class=" container d-flex flex-row justify-content-between p-5 ">
    <div class="">
        <button class="btn border-primary text-uppercase text-light">sign-up now</button>
    </div>
    <div class="d-flex flex-row ">
        <span class="text-primary text-uppercase">follow us</span>
        <ul class="d-flex flex-row">
            <li class="border" v-for="el in icons"><img :src="el.image" :alt="el.text"></li>
        </ul>
    </div>
</div>
  </div>
</template>

<script>
    export default {
        name: "bottomFooter",
        data(){
    return {
        icons :[
            {
                image: "/src/assets/images/footer-facebook.png",
                text: "facebook"
            },
            {
                image: "/src/assets/images/footer-twitter.png",
                text: "twitter"
            },
            {
                image: "/src/assets/images/footer-youtube.png",
                text: "youtube"
            },
            {
                image: "/src/assets/images/footer-pinterest.png",
                text: "pinterest"
            },
            {
                image: "/src/assets/images/footer-periscope.png",
                text: "periscope"
            }
        ]
    }
    }
    
  }
</script>

<style lang="scss" scoped>

</style>