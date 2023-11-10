<template>
   
    <div class="card">
        <img :src="img"  :alt="title">
        
        </div>
   
</template>

<script>
export default {
    name: 'cardComics',
    props: {
        img: String,
        title: String,
    }

}
</script>

<style lang="scss" scoped>
.card{
    width: calc(100% / 6);
    height: 100px;
}
</style>