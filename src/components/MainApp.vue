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
main {
  width: 100%;

}

</style>
