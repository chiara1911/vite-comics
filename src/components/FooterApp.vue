<template>
  <footer>
    <topFooter />
  <bottomFooter />
  
</footer>
</template>

<script>
import topFooter from "./footer/topFooter.vue";
import bottomFooter from "./footer/bottomFooter.vue"
export default {
  name: "FooterApp",

  components: {
    topFooter,
    bottomFooter,
  },

 
};
</script>

<style lang="scss" scoped></style>
