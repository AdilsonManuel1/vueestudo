<template>
<div>
        <h2>Descricao da pessoa</h2>
        <info />
        <pictore/>
       
</div>
</template>
<script>

import info from './info.vue'
import pictore from'./picture.vue'

export default {
 name:"pessoa",
  components:{
    info,
    pictore,
    
 },
 data(){
 return{
       nome:"Adilson"
 }
 }

}
</script>
