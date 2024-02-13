<template>
    <img :src='imageCaminho'  :alt='desc'>
</template>

<script>

export default{
    name:'Picture',
    data(){
        return{
            imageCaminho:'/img/logo.png',
            desc:"Adilson Liindo"
        }
    }
}

</script>
