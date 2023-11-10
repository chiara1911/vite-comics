<template>
  <div id="top-main" class="bg-dark pt-2">
    <div id="hero-img">
      hello
    </div>
    <div class="container">
      <div class="row">
        <div class="col-lg-2 col-md-3" v-for="comic in comics">
          <cardComics :img="comic.thumb" :title="comic.series" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { comicsDc } from "../../data/dc-comics";
import cardComics from "./cardComics.vue";
export default {
  name: "topMain",
  components: {
    cardComics,
  },
  data() {
    return {
      comics: comicsDc,
    };
  },
};
</script>

<style lang="scss" scoped>
#top-main {
  height: 400px;
  width: 100%;
}

img{
  object-fit: contain;
  width: 100%
}
#hero-img{
    background-image: url(../../assets/images/jumbotron.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 300px;
}
</style>
