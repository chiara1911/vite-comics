<template>
  <div class="container p-3">
    <div class="row">
      <div class="d-flex justify-content-between">
        <div class="col-5">
          <div class="row">
            <div class="col-4">
              <ul>
                <h4 class="text-uppercase text-light">dc comics</h4>
                <li v-for="comic in comics" class="text-light"><a href="#">{{comic}}</a></li>
              </ul>
              <ul>
                <h4 class="text-uppercase text-light">shop</h4>
                <li v-for="shopEl in shop" class="text-light"><a href="#">{{shopEl}}</a></li>
              </ul>
            </div>

            <div class="col-4">
              <ul>
                <h4 class="text-uppercase text-light">dc</h4>
                <li v-for="dcEl in dc" class="text-light"><a href="#">{{dcEl}}</a></li>
              </ul>
            </div>
            <div class="col-4">
              <ul>
                <h4 class="text-uppercase text-light">sites</h4>
                <li v-for="sitesEl in sites" class="text-light">
                  <a href="#" >{{ sitesEl }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-7 d-flex justify-content-end position-relative ">
          <img src="/src/assets/images/dc-logo-bg.png" alt="dc-logo-bg" class="position-absolute"/>
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
      shop: ["shop DC", "Shop DC Collectibles"],

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

<style lang="scss" scoped></style>
