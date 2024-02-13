<template>

<div class="conteudo">
  <div class="animesdesenho">
   <animesComponents :caminhoImagem='caminhoImagemEren' :descc='desc'/> 
   <animesComponents :caminhoImagem='caminhoImagemmashele' :descc='desc'/> 
   <animesComponents :caminhoImagem='caminhoImagemtommy' :descc='desc'/> 
   <animesComponents :caminhoImagem='caminhoImagemtommy' :descc='desc'/> 

  </div>

      <CenterImage/>
     
</div>
</template>



<script>
import animesComponents from './components/animesComponents.vue'
import CenterImage from './components/CenterImage.vue'



export default{
   name:'App',
  components: {
        animesComponents,
      CenterImage,



  },
  data(){
    return{
        caminhoImagemEren:'/img/eren.jpg',
        caminhoImagemmashele:'/img/mashele.jpg',
        caminhoImagemtommy:'/img/tommy.jpg',


        desc:"Tentei",
    }
  }
  
}

</script>

<style scoped>
*{
  margin: 0px,
}
.conteudo{
background-color: #9b3541;
}
.animesdesenho{
  display: flex;
  margin-bottom: 10px;
  padding-top: 10px;

  justify-content: space-around;
}
</style>>


