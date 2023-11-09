

<template>
 <HeaderApp />
 <MainApp />
 <FooterApp />
  
  
</template>


<script >
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';
import bottomMain from './components/main/bottomMain.vue';

export default {
  name: 'App',
  components: {
    HeaderApp,
    MainApp,
    bottomMain,
    FooterApp
  },
  data(){
    return {

    }
  },
  methods:{

  }
 
}
</script>



<style scoped>


</style>
