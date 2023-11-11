<template>
  <div id="top-footer" >
    <div class="container ">
      <div class="row py-2">
        <div
          class="d-flex justify-content-between position-relative overflow-hidden"
        >
        
            <div class="row">
              <div class="col-4">
                <ul>
                  <h4 class="text-uppercase text-light">dc comics</h4>
                  <li v-for="comic in comics" class="text-light">
                    <a href="#">{{ comic }}</a>
                  </li>
                </ul>
                <ul>
                  <h4 class="text-uppercase text-light">shop</h4>
                  <li v-for="shopEl in shop" class="text-light">
                    <a href="#">{{ shopEl }}</a>
                  </li>
                </ul>
              </div>

              <div class="col-4">
                <ul>
                  <h4 class="text-uppercase text-light">dc</h4>
                  <li v-for="dcEl in dc" class="text-light">
                    <a href="#">{{ dcEl }}</a>
                  </li>
                </ul>
              </div>
              <div class="col-4">
                <ul>
                  <h4 class="text-uppercase text-light">sites</h4>
                  <li v-for="sitesEl in sites" class="text-light">
                    <a href="#">{{ sitesEl }}</a>
                  </li>
                </ul>
              </div>
            </div>
        

          <div class="position-absolute" id="footer-img">
            <img src="/src/assets/images/dc-logo-bg.png" alt="dc-logo-bg" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "topFooter",

  data() {
    return {
      comics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Video",
        "News",
      ],
      shop: ["Shop DC", "Shop DC Collectibles"],

      dc: [
        "Terms Of Use",
        "Privacy policy (New)",
        "Ad Choice",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],

      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
};
</script>

<style lang="scss" scoped>
#top-footer {
  background-image: url(../../assets/images/footer-bg.jpg);
  height: 350px; 
  #footer-img {
  margin-left: 700px;
  margin-top: -32px;

 }
 a{
  color: grey;
 }
}

@media screen and (max-width: 992px){
  
  #footer-img{
    display: none;
  }
}


</style>
