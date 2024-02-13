<template>
        <div class="personagem">
        <img :src="caminhoImagem" :alt="descc">
        <p>Eren</p>
 
</div>
</template>

<script>
export default{
    name:'animesComponents',
    props:['caminhoImagem','descc'], // isso literalemte salvou me a noite, serve para passar parametros que vás usar em outros componentes.

   
    }


</script>

<style scoped>

.personagem{
    width: 150px;
    height: 150px;
    border-radius: 50%;
    overflow: hidden;
}
.personagem img{
   width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>
