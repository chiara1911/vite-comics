<template>
  <main>
    <topMain />
      <bottomMain />
   
  </main>
</template>

<script>
import bottomMain from "./main/bottomMain.vue";
import topMain from "./main/topMain.vue";

export default {
  name: "MainApp",
  components: {
    bottomMain,
    topMain,
    
  },
};
</script>

<style lang="scss">
#top-main {
  background-color: black;
}
#bottom-main {
  background-color: rgb(0, 115, 255);
}
</style>
