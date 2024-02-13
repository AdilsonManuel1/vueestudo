<template>
    <h1>Meu nome é {{nome}}</h1>
</template>

<script>


export default{
    name:'lifeCycle',
    data(){
 return{
           nome:"n"
        }
    },
    // lifeCycle hocks posso determinar cada coisa com um tempo.
    created(){
        setTimeout(()=>{
            this.nome="Manuel"
        },1000)
        
    },
    mounted(){
        this.nome= 'Adiware';
    }
}
</script>
