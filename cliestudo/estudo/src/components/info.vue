<template>
<div class="teste">
         <p v-if="trabalha">Estou a trabalhar com desevolvimento frontend com Vue</p>
         <p v-else outro> Estou estudando e batalhando</p>

         <p v-if="pais==='Angola'">
            <ul>
                <li>Luanda</li>
                <li>Benguela</li>
                <li>Huambo</li>
                <li>Benguela</li>
            </ul>
         </p>
         <p v-else> <input type="text" placeholder="Insira o Pais">  </p>
        <h4> Tecnologias que uso </h4>
        <ul v-for="(tecnologia, index) in tecnologias" :key="index"> <!-- sem um index, funciona mas pode mostrar erro, entãp adicione um index, depois passar na key !-->
           <li>{{tecnologia}}</li>
        </ul>

        <h2>Tecnologias Front end</h2>
        <ul>
            <li v-for="front in fronted_tec" :key="front.id"> <!-- aqui é quase a mesma coisa que fiz acima!-->
                {{front.tec}}
            </li>
        </ul>
        <p> para aceder <a v-bind:href="link" target="_bank"> acess</a> </p>
        <button @click="mostrarEma">Mostrar Emial</button>
        <p v-show="mostrarEmail" >Meu emial: {{email}}</p>
</div>
</template>

<script>


export default {
    name:"info",
    
    data(){
        return{
            trabalha:false,
             pais:"Angola",
             outro:"",
             email:"Adilson.manuel",
             mostrarEmail: false,
             link:"https://google.com",
             tecnologias:[
                'JavaScript',
                'Node',
                'Flutter',
             ],
             fronted_tec:[
                {id:1, tec:"Vue"},
                {id:2, tec:"Angular"},
                {id:3, tec:"React"},


             ]
        };
                
    },

   // this.pais = prompt("Insira o teu pais ");
   methods:{
        mostrarEma(){
            this.mostrarEmail= !this.mostrarEmail;
        }
    },

};



</script>

<style>

.teste{
    background-color: red;
    border-radius: 20px;
    padding-left: 30px;
    padding: 30px;
    width: 50%;
    color: white;
    font-weight: bold;
}

</style>