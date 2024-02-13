<template>
   <div class="imagemCenter">
     <img :src='imagemCaminho' :alt="desc">
   </div>
        
   
</template>

<script>


export default {
    name:'CenterImage',
    data(){
        return{
            imagemCaminho:'/img/eren.jpg',
            desc:"Ola",
        }
    }
}
</script>

<style>
.imagemCenter{
    width: 60%;
    margin-left: auto;
    margin-right: auto;
    
}
.imagemCenter img{
    width: 100%;
}
</style>
