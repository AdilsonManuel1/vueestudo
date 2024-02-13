<template>
<div>
  Eu quero Falar que você é importante
 <primeeirocomponente/>
    <lifeCycle />
    <pessoa/>
 Porem você também
  <HelloWorld/>

</div>


</template>

<script>
import primeeirocomponente from './components/primeirocomponente.vue'
import HelloWorld from './components/HelloWorld.vue'
import lifeCycle from './components/lifeCycle.vue'
import pessoa from './components/pessoa.vue'




export default{
  name:'App',
  components:{
    primeeirocomponente,
    HelloWorld,
    lifeCycle,
    pessoa,

  }
}
</script>
