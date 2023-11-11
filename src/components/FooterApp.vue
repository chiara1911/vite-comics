<template>
  <footer>
    <topFooter />
    <bottomFooter />
  </footer>
</template>

<script>
import topFooter from "./footer/topFooter.vue";
import bottomFooter from "./footer/bottomFooter.vue";
export default {
  name: "FooterApp",

  components: {
    topFooter,
    bottomFooter,
  },
};
</script>

<style lang="scss" scoped>
footer {
  width: 100%;
  a {
    font-size: 0.6rem;
    color: grey;
    text-decoration: none;
  }
  img {
    width: 100%;
    object-fit: cover;
  }
  h4 {
    font-size: 0.8rem;
  }
}

@media screen and (min-width: 767px) {
  footer {
    font-size: 0.7rem;
  }
}
</style>
