<template>
  <footer>
    <topFooter />
  
  <div id="bottomFooter" class="d-flex flex-row justify-content-between p-5">
    <div>
        <button class="btn border-dark text-uppercase ">sign-up now</button>
    </div>
    <div class="d-flex flex-row ">
        <span>follow us</span>
        <ul class="d-flex flex-row">
            <li class="border" v-for="el in icons"><img :src="el.image" :alt="el.text"></li>
        </ul>
    </div>
  </div>
</footer>
</template>

<script>
import topFooter from "./footer/topFooter.vue";
export default {
  name: "FooterApp",

  components: {
    topFooter,
  },

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
};
</script>

<style lang="scss" scoped></style>
