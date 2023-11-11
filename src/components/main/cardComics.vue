<template>
   
    <div class="card-wrapper">
        <div class="img-card overflow-hidden">
            <img :src="img"  :alt="title">
        </div>
       
        <h5 class="text-uppercase pt-1">{{ title }}</h5>
        
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
.card-wrapper{
    width: 100px;
}
h5{
    font-size: 0.6rem;
    color: white;
}
.img-card{
    width: 150px;
    height: 150px;
    cursor: pointer;
}
img{
    width: 100%;

}
</style>