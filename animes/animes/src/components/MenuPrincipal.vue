<template>
<div>
        <nav :class="{ 'nav-blue': corAzul }"> <!-- Esse código é simples mas complicado, aqui criei uma class css nac-blue, depois passei uma variavel corAzul para controlar o estado. -->
        <ul>
            <li> <a @click="corMuda">Assistir Agora</a> </li>
            <li> <button @click="corMuda">Contacto</button> </li>
        </ul>
    </nav>
</div>
</template>

<script>
export default{
    name:'MenuPrincipal',
    data(){
      return{
          corAzul:false,
      }
    },

    methods:{
        corMuda(){
          this.corAzul = !this.corAzul;
            
        }
    }
}
</script>

<style scoped>
*{
    padding: 0;
    margin: 0;

}
nav{
    background-color: #9b3541;
    padding: 15px;
    width: 50%;
    margin-left: auto;
    margin-right: auto;
 
}
nav ul{
   display: flex;
 
}
nav ul li{
   list-style: none;
   color: yellow;
   padding: 10px;
   cursor: pointer;
}
.nav-blue {
  background-color: blue;
}

/*
nav:active{
    background-color: blue;
}*/
</style>