<template>
    <div id="top-main" class="bg-dark">       
        <ul class="d-flex flex-row">
          <li v-for="comic in comics" >
            <cardComics :img="comic.thumb" :title="comic.series"/>
          </li>
        </ul>          
      </div>
</template>

<script>
import { comicsDc } from '../../data/dc-comics';
import cardComics from './cardComics.vue';
    export default {
        name: "topMain",
         components:{
          cardComics
         },
        data(){
          return {
            comics : comicsDc,
           
          }
          
        }
    }
</script>

<style lang="scss" scoped>
#top-main{
  height: 200px;
  width: 100%;
}

</style>